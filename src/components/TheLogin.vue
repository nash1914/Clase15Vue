<template>
  <v-container class="d-flex justify-center">
    <v-form ref="form" v-model="valid" lazy-validation>
      <v-card elevation="2" min-width="500">
        <v-container>
          <v-card-text>
            <h1 class="text-center mb-10">Inicio de Seccion</h1>
            <v-row>
              <v-col cols="12">
                <v-text-field
                  v-model="email"
                  :rules="emailRules"
                  label="E-mail"
                  required
                  outlined
                ></v-text-field>
              </v-col>
              <v-col cols="12">   
                <v-text-field
                  v-model="password"
                  :append-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
                  :rules="[rules.required, rules.min]"
                  :type="show1 ? 'text' : 'password'"
                  name="input-10-1"
                  label="Password"
                  hint="At least 8 characters"
                  @click:append="show1 = !show1"
                  outlined
                ></v-text-field>
              </v-col>
            </v-row>
          </v-card-text>
        </v-container>

        <v-card-actions>
          <v-row>
            <!-- class="d-flex justify" -->
            <v-col cols="12" md="6">
              <v-btn
                block
                rounded
                :disabled="!valid"
                color="success"
                class="mr-4"
                @click="ingresar"
              >
                Ingresar
              </v-btn>
            </v-col>
            <v-col cols="12" md="6">
              <v-btn block rounded color="error" class="mr-4" @click="reset">
                Reiniciar
              </v-btn>
            </v-col>
          </v-row>
        </v-card-actions>
      </v-card>
    </v-form>
  </v-container>
</template>

<script>
import axios from "axios";

export default {
  data: () => ({
    password: "",
    mensaje: "",
    valid: true,
    show1: false,
    name: "TheLogin",
    email: "",
    emailRules: [
      (v) => !!v || "E-mail is required",
      (v) => /.+@.+\..+/.test(v) || "E-mail must be valid",
    ],
    rules: {
      required: (value) => !!value || "Required.",
      min: (v) => v.length >= 8 || "Min 8 characters",
      emailMatch: () => `The email and password you entered don't match`,
    },
  }),

  methods: {
    ingresar() {
      // Va a realizar una peticion axios. Peticion http a nuestro Backend
      axios
        .post("http://localhost:4000/api/create-student/", {
          // se envian dos parametros
          email: this.email,
          password: this.password,
        })
        .then((respuesta) => {
          return respuesta.data;
        })
        .then((data) => {
          localStorage.setItem("token", data.tokenReturn); // Almacenamos el token en el local storage
          this.$router.push({ name: "Admin" }); //Agregamos, o lo mandamos a la vista del Admin
        })
        .catch((err) => {
          // Hacemos un manejo de los errores, solamente imprimiendo en console
          this.mensaje = null;
          if ([404, 401].includes(err.response.status)) {
            this.mensaje = "El correo o la contraseña son incorrectos";
            console.log(this.mensaje);
          } else {
            //en caso de error 500
            this.mensaje = "ocurrio un error interno";
            console.log(this.mensaje);
          }
        });
    },
    reset() {
      this.$refs.form.reset();
    },
  },
};
</script>
