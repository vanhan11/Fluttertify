<template>
  <v-row>
    <v-col class="text-center">
        <TopBar/>

         <v-card class="mx-auto mt-5" max-width="480" v-for="(data, id) in datas" :key="id">
          <v-row>
            <v-col cols="3" sm="3" class="">
              <a :href="data.link" target="_blank">
                 <v-img
                    class="rounded ml-2"
                    height="100px"
                    width="100px"
                    :src="data.thumbnail"
                  >
                  </v-img>
              </a>
            </v-col>
            <v-col cols="9" sm="9" class="text-left">
               <v-card elevation="0" class="pr-2">
                  <p class="font-color text-left font-weight-bold text-caption">
                    <a :href="data.link" target="_blank" rel="noopener noreferrer">{{ data.title }}</a>
                  </p>
                  <p class="font-desc">{{ data.description }}</p>
                </v-card>
            </v-col>
          </v-row>
        </v-card>
        <BottomNavigation />
    </v-col>
  </v-row>
</template>

<script>
  import axios from 'axios'

  export default {
    async asyncData() {
      const {
        data
      } = await axios.get('https://api-berita-indonesia.vercel.app/antara/terbaru/')
      return {
        datas: data['data']['posts']
      }
    }
  }

</script>
