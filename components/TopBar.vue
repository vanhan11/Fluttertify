<template>
    <v-app-bar
        flat
        fixed 
        app
        color="white"
        :max-width="480"
        height="50"
        class="css"
    >
    <v-toolbar-title class="font-weight-bold">Fluttertify</v-toolbar-title>
    <v-spacer />
    <v-btn 
        small
        outlined
        class="text-caption"
    >
        <v-icon small left>
        mdi-earth
        </v-icon>   
        Id
    </v-btn>
    <v-btn 
        flat
        small
        color="#FFB230"
        class="ml-2 text-xs font-weight-medium"
    >
        <span class="font-4">Masuk/Daftar</span> 
    </v-btn>
    </v-app-bar>
</template>
<style>
.css{
    width: 480px;
    position: fixed;
    top: 0;
    margin-left: auto;
    margin-right: auto;
    align-items: center;
    justify-content: center;
}
.font-4{
    color: rgb(255, 255, 255);
    font-size: 10px;
  }
</style>