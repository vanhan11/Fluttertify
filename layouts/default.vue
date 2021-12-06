<template>
  <v-app app>
    

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    

  </v-app>
</template>

<style>
.fixed-container{
    position: fixed;
    height: 100vh;
    width: 100vw;
    z-index: 999;
    top: 0;
    left: 0;
    opacity: 0;
    pointer-events: none;
    transition: all .3s;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>