<template>
    <v-app-bar
        flat
        fixed 
        app
        color="white"
        :max-width="480"
        class="css"
    >
    <v-toolbar-title>Fluttertify</v-toolbar-title>
    <v-spacer />
    <v-btn 
        outlined
        color="success"
    >
        <v-icon left>
        mdi-pencil
        </v-icon>   
        Edit
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
</style>