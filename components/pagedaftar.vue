<template>
  <v-row>
    <v-col class="text-center">
      <TopBar />
      <v-card class="mx-auto" max-width="450" flat>
        <v-tabs class="mx-auto text-capitalize " max-width="450" fixed-tabs color="#F27128">
          <v-tab class=" text-capitalize ">
            Polis Saya
          </v-tab>
          <v-tab class=" text-capitalize ">
            Status Klaim
          </v-tab>
          <v-tab-item v-for="n in 2" :key="n">
            <v-container class="mt-10">
              <v-carousel :show-arrows="false" delimiter-icon="mdi-minus" cycle height="400" hide-delimiter-background>
                <v-carousel-item v-for="(slide, i) in slides" :key="i">
                  <v-sheet height="100%">
                    <v-row class="fill-height" align="center" justify="center">
                      <div class="text-h2">
                        {{ slide }} Slide
                      </div>
                    </v-row>
                  </v-sheet>
                </v-carousel-item>
              </v-carousel>
            </v-container>
              <v-btn block large color="#F27128" class=" white--text text-capitalize rounded-lg mt-15 ">
                Daftar Sekarang
              </v-btn>
              <v-btn block large color="#F8F8F8" class=" indigo--text text-capitalize rounded-lg mt-5 ">
                Masuk
              </v-btn>
          </v-tab-item>
        </v-tabs>
      </v-card>
    </v-col>
    <BottomNavigation />
  </v-row>
</template>


<script>
  export default {
    data() {
      return {
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
      }
    },
  }

</script>
