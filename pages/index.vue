<template>
  <div>
    <v-row max-width="480">
      <v-col class="text-center">
        <TopBar />
        <v-card class="mx-auto" max-width="480" elevation="1">
          <v-carousel cycle width="480" height="180" hide-delimiter-background show-arrows-on-hover>
            <v-carousel-item v-for="(slide, i) in slides" :key="i">
              <v-sheet :color="colors[i]" height="110%">
                <v-row class="fill-height" align="center" justify="center">
                  <div class="text-h6">
                    {{ slide }} Slide
                  </div>
                </v-row>
              </v-sheet>
            </v-carousel-item>
          </v-carousel>
          <v-row no-gutters class="overflow-auto">
            <v-col
              cols="12"
              sm="12"
            >
              <v-card
                class="pa-2"
                tile
              >
                <v-row no-gutters>
                  <v-col
                    cols="3"
                    sm="3"
                    class="pa-2"
                    v-for="(router, id) in routers"
                    :key="id"
                  >
                    <nuxt-link class="font" :to="router.to">
                      <v-card
                        tile
                        text
                        elevation="0"
                      > 
                        <v-icon :color="router.color" large>{{ router.icon }}</v-icon><br>
                        <span class="font">{{ router.title }}</span>
                      </v-card>
                    </nuxt-link>
                  </v-col>
                </v-row>
              </v-card>
            </v-col>
          </v-row>
        </v-card>
        <v-card class="mx-auto mt-2" max-width="480" elevation="1">
          <p class="font-color text-left ml-3 pt-2 font-weight-bold text-caption">Kenapa Fluttertify?</p>
          <v-row>
            <v-col
              cols="4"
              sm="4"
            >
              <v-card elevation="0" color="#F6F9FF" class="pl-2 ml-2" height="50">
                <v-row class="m-1">
                  <v-col cols="3" sm="3">
                     <v-icon color="#FFB230" left>mdi-scale-unbalanced</v-icon>
                      
                  </v-col>
                   <v-col cols="9" sm="9">
                     <p class="font-2 font-weight-medium text-left">Bandingkan Dengan Mudah</p>
                  </v-col>
                </v-row>
              </v-card>
            </v-col>
              <v-col
              cols="4"
              sm="4"
            >
              <v-card elevation="0" color="#F6F9FF" class="pl-5" height="50">
                <v-row class="m-1">
                  <v-col cols="3" sm="3">
                     <v-icon color="#FFB230" left>mdi-information-outline</v-icon>
                      
                  </v-col>
                   <v-col cols="9" sm="9">
                     <p class="font-2 font-weight-medium text-left">Informasi Transparan</p>
                  </v-col>
                </v-row>
              </v-card>
            </v-col>
              <v-col
              cols="4"
              sm="4"
            >
              <v-card elevation="0" color="#F6F9FF" class="pl-2 mr-2" height="50">
                <v-row class="m-1">
                  <v-col cols="3" sm="3">
                     <v-icon color="#FFB230" left>mdi-timer-outline</v-icon>
                      
                  </v-col>
                   <v-col cols="9" sm="9">
                     <p class="font-2 font-weight-medium text-left">Pembelian Online & Praktis</p>
                  </v-col>
                </v-row>
              </v-card>
            </v-col>
          </v-row>
        </v-card>
        <v-card class="mx-auto" max-width="480" elevation="0">
          <p class="font-color text-left mt-5 ml-2 pt-2 font-weight-bold text-caption">Jelajahi Produk Fluttertify</p>
        </v-card>
        <v-card  class="mx-auto" max-width="480">
          <v-row>
            <v-col cols="3" sm="3" class="">
              <nuxt-link to="">
                 <v-img
                    class="rounded ml-2"
                    height="100px"
                    width="100px"
                    src="https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg"
                  >
                  </v-img>
              </nuxt-link>
            </v-col>
            <v-col cols="9" sm="9" class="text-left">
               <v-card elevation="0">
                  <v-card-title class="font-color text-left font-weight-bold text-caption">
                    San Francisco
                  </v-card-title>
                  <v-card-subtitle class="font-2">Mon, 12:30 PM, Mostly sunnydwdwdww</v-card-subtitle>
                </v-card>
            </v-col>
          </v-row>
        </v-card>
         <v-card  class="mx-auto mt-5" max-width="480">
          <v-row>
            <v-col cols="3" sm="3" class="">
              <nuxt-link to="">
                 <v-img
                    class="rounded ml-2"
                    height="100px"
                    width="100px"
                    src="https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg"
                  >
                  </v-img>
              </nuxt-link>
            </v-col>
            <v-col cols="9" sm="9" class="text-left">
                <v-card elevation="0">
                  <v-card-title class="font-color text-left font-weight-bold text-caption">
                    San Francisco
                  </v-card-title>
                  <v-card-subtitle class="font-2">Mon, 12:30 PM, Mostly sunnydwdwdww</v-card-subtitle>
                </v-card>
            </v-col>
          </v-row>
        </v-card>
         <v-card  class="mx-auto mt-5" max-width="480">
          <v-row>
            <v-col cols="3" sm="3" class="">
              <nuxt-link to="">
                 <v-img
                    class="rounded ml-2"
                    height="100px"
                    width="100px"
                    src="https://cdn.pixabay.com/photo/2020/07/12/07/47/bee-5396362_1280.jpg"
                  >
                  </v-img>
              </nuxt-link>
            </v-col>
            <v-col cols="9" sm="9" class="text-left">
                <v-card elevation="0">
                  <v-card-title class="font-color text-left font-weight-bold text-caption">
                    San Francisco
                  </v-card-title>
                  <v-card-subtitle class="font-2">Mon, 12:30 PM, Mostly sunnydwdwdww</v-card-subtitle>
                </v-card>
            </v-col>
          </v-row>
        </v-card>
        <br>
        <BottomNavigation />
      </v-col>
    </v-row>
    <!-- <v-row justify="right" align="right">
      <v-col class="text-right button">
         <v-btn
            elevation="2"
            fab
            right
          ></v-btn>
      </v-col>
    </v-row> -->
  </div>
</template>

<script>
  export default {
    data () {
      return {
        colors: [
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ],
        slides: [
          'First',
          'Second',
          'Third',
          'Fourth',
          'Fifth',
        ],
        routers: [
          {
            icon: 'mdi-cellphone',
            color: '#4863FF',
            title: 'Smartphone',
            to: '/asuransi/smartphone'
          },
          {
            icon: 'mdi-car',
            color: '#60CAC1',
            title: 'Polis',
            to: '/asuransi/car'
          },
          {
            icon: 'mdi-motorbike',
            color: '#FF7500',
            title: 'Motor',
            to: '/asuransi/motor'
          },
          {
            icon: 'mdi-medical-bag',
            color: '#F08D87',
            title: 'Kesehatan',
            to: '/asuransi/kesehatan'
          },
          {
            icon: 'mdi-cash-multiple',
            color: '#BD9ADE',
            title: 'Santunan Tunai',
            to: '/asuransi/tunai'
          },
           {
            icon: 'mdi-heart-pulse',
            color: '#D94A3C',
            title: 'Jiwa',
            to: '/asuransi/jiwa'
          },
           {
            icon: 'mdi-virus',
            color: '#8EC2A2',
            title: 'Penyakit Tropis',
            to: '/asuransi/virus'
          },
           {
            icon: 'mdi-bag-suitcase',
            color: '#76BACD',
            title: 'Perjalanan',
            to: '/asuransi/perjalanan'
          },
        ]
      }
    },
  }
</script>