<template>
    <v-bottom-navigation 
        app
        fixed
        max-width="480"
        class="csss"
    >
    <v-btn v-for="(router, id) in routers"
    :key="id" :to="router.to">
        <span>{{ router.title }}</span>

        <v-icon>{{ router.icon }}</v-icon>
    </v-btn>
    </v-bottom-navigation>
</template>
<style>
.csss{
    width: 480px;
    left: 0;
    right: 0;
    margin-left: auto;
    margin-right: auto;
    align-items: center;
    justify-content: center;
}
</style>
<script>
export default {
  data () {
    return {
      routers: [
        {
          icon: 'mdi-home',
          title: 'Home',
          to: '/'
        },
        {
          icon: 'mdi-shield',
          title: 'Polis',
          to: '/polis'
        },
        {
          icon: 'mdi-plus-circle',
          title: 'Klaim',
          to: '/klaim'
        },
        {
          icon: 'mdi-bell-ring',
          title: 'Notifikasi',
          to: '/notifikasi'
        },
        {
          icon: 'mdi-account-circle',
          title: 'Akun',
          to: '/akun'
        },
      ]
    }
  }
}
</script>