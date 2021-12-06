<template>
  <v-row justify="center" align="center">
    <v-col class="text-center css">
      <TopBar />
      <v-card class="mt">
        <v-carousel cycle width="480" height="240" hide-delimiter-background show-arrows-on-hover>
          <v-carousel-item v-for="(slide, i) in slides" :key="i">
            <v-sheet :color="colors[i]" height="110%">
              <v-row class="fill-height" align="center" justify="center">
                <div class="text-h2">
                  {{ slide }} Slide
                </div>
              </v-row>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
        <v-row no-gutters>
          <v-col
            cols="12"
            sm="12"
          >
            <v-card
              class="pa-2"
              outlined
              tile
            >
              One of three columns
            </v-card>
          </v-col>
        </v-row>
      </v-card>
      <v-card>
        
      </v-card>
    </v-col>
    <BottomNavigation />
  </v-row>
</template>
<style>
  .css {
    width: 480px;
    margin-left: auto;
    margin-right: auto;
    align-items: center;
    justify-content: center;
  }
  .mt{
    margin-top: 65px;
  }
</style>
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
      }
    },
  }
</script>