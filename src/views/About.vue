<template>
  <div>
    <div class="d-flex justify-center"></div>
    <v-row class="d-flex" justify="center">
      <v-menu v-model="showMenu" absolute offset-y style="max-width: 600px">
        <template v-slot:activator="{ on, attrs }">
          <v-card
            class="portrait"
            img="https://i.ibb.co/vqMjn8j/BAnner-CAtalogo.jpg"
            height="300"
            width="600"
            v-bind="attrs"
            v-on="on"
          ></v-card>
        </template>

        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index">
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-row>
    <br />

    <!--  -->

    <v-layout class="d-flex justify-space-around mb-6">
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/q0H3fHR/imagen-2021-10-20-084819.png"
          ></v-img>
          <v-card-text>
            <div>Play Station 4</div>
            <p class="text-h4 text--primary">
              Marvel Spiderman
            </p>
            <p>Genero</p>
            <div class="text--primary">
              Es un videojuego de acción y aventuras con un estilo jugable de
              mundo abierto<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal13 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal13"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  El juego plantea una jugabilidad similar a lo visto en la saga
                  de Batman Arkham, ya que ofrece mecánicas de sigilo con las
                  que ir abatiendo a los enemigos uno a uno (o de varios en
                  varios) entremezclándolas con elementos de acción y combate
                  directo de control de multitudes.’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal13 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>

      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/7VzBzRx/Bloodbourne-banner.webp"
          ></v-img>
          <v-card-text>
            <div>Play Station 4</div>
            <p class="text-h4 text--primary">
              Bloodbourne
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal12 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal12"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal12 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/cD6pdVD/horizon-banner.jpg"
          ></v-img>
          <v-card-text>
            <div>Play Station 4</div>
            <p class="text-h4 text--primary">
              Horizon Forbidden West
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal11 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal11"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal11 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/x1RZ5vh/Kena-banner.webp"
          ></v-img>
          <v-card-text>
            <div>Play Station 4</div>
            <p class="text-h4 text--primary">
              Kena Bridge Of Spirits
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal10 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal10"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal10 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
    </v-layout>

    <!-- OTro Layout -->
    <v-layout class="d-flex justify-space-around mb-6">
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/0ZjSv14/juego-xbox-play-anywhere-gears-5-pc-xbox-one-cover.jpg"
          ></v-img>
          <v-card-text>
            <div>Xbox ONE</div>
            <p class="text-h4 text--primary">
              Gear 5
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal9 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal9"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal9 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/Q62rLNB/halo-infinite-pgr9.jpg"
          ></v-img>
          <v-card-text>
            <div>Xbox ONE</div>
            <p class="text-h4 text--primary">
              Halo Infinite
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal8 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal8"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal8 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/GTWnBdk/490104-forza-motorsport-7-windows-apps-front-cover.jpg"
          ></v-img>
          <v-card-text>
            <div>Xbox ONE</div>
            <p class="text-h4 text--primary">
              Forza Motorsport
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal7 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal7"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal7 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/LgMPLKx/1291414.png"
          ></v-img>
          <v-card-text>
            <div>Xbox ONE</div>
            <p class="text-h4 text--primary">
              Killer Instinct
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal6 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal6"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal6 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
    </v-layout>

    <!-- Otro Layout -->

    <v-layout class="d-flex justify-space-around mb-6">

      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/GMryz5N/The-Legend-of-Zelda-Breath-of-the-Wild.jpg"
          ></v-img>
          <v-card-text>
            <div>Nintendo</div>
            <p class="text-h4 text--primary">
              The Legend Of Zelda Breath of the Wild
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal5 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal5"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Origin
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal5 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/RHgrhhP/SQ-NSwitch-Super-Mario-Odyssey-Alt01-image500w.jpg"
          ></v-img>
          <v-card-text>
            <div>Nintendo</div>
            <p class="text-h4 text--primary">
              Super Mario Odyssey
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal3 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal3"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal3 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/dtpC3Q0/c67a-metroid-dread.jpg"
          ></v-img>
          <v-card-text>
            <div>Nintendo</div>
            <p class="text-h4 text--primary">
              Metroid Dread
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal2 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal2"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal2 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
      <v-flex>
        <v-card class="mx-auto" max-width="300">
          <v-img
            height="250"
            src="https://i.ibb.co/hDR6zGK/9fa229169c78622c3ad4f19589360cdd0a5ed5d1.jpg"
          ></v-img>
          <v-card-text>
            <div>Nintendo</div>
            <p class="text-h4 text--primary">
              Monster Hunter Rise
            </p>
            <p>Genero</p>
            <div class="text--primary">
              relating to or dependent on charity; charitable.<br />
              "an eleemosynary educational institution."
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn text color="teal accent-4" @click="reveal1 = true">
              Learn More
            </v-btn>
          </v-card-actions>

          <v-expand-transition>
            <v-card
              v-if="reveal1"
              class="transition-fast-in-fast-out v-card--reveal"
              style="height: 100%;"
            >
              <v-card-text class="pb-0">
                <p class="text-h4 text--primary">
                  Resumen
                </p>
                <p>
                  late 16th century (as a noun denoting a place where alms were
                  distributed): from medieval Latin eleemosynarius, from late
                  Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’
                </p>
              </v-card-text>
              <v-card-actions class="pt-0">
                <v-btn text color="teal accent-4" @click="reveal1 = false">
                  Close
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-expand-transition>
        </v-card>
      </v-flex>
      <!--  -->
    </v-layout>
  </div>

  <!--  -->
</template>

<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}
</style>

<script>
export default {
  data: () => ({
    showMenu: false,
    items: [
      { title: "Juegos PlayStation" },
      { title: "Juegos Xbox" },
      { title: "Juegos Nintendo" },
    ],
    reveal: false,
    reveal1: false,
    reveal2: false,
    reveal3: false,
    reveal4: false,
    reveal5: false,
    reveal6: false,
    reveal7: false,
    reveal8: false,
    reveal9: false,
    reveal10: false,
    reveal11: false,
    reveal12: false,
    reveal13: false,
  }),
};
</script>
