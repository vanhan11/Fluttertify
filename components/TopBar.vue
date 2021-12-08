<template>
    <v-app-bar
        elevation="0"
        fixed 
        app
        color="white"
        :max-width="480"
        height="50"
        class="css-topbar"
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
        small
        color="#FFB230"
        class="ml-2 text-xs font-weight-medium"
    >
        <span class="font-4">Masuk/Daftar</span> 
    </v-btn>
    </v-app-bar>
</template>