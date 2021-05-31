<template>
  <v-app dark>
    <!-- <v-app-bar fixed app> </v-app-bar> -->
    <v-main>
        <nuxt />

    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: '',
    }
  },
}
</script>

<style>

.font-lulu {
  font-family: 'Lulu', sans-serif;
}
.font-avenir {
  font-family: 'Avenir', sans-serif;
}
.v-slide-group__content.v-tabs-bar__content {
    background-color: black;
}
.fs-0-7{
  font-size: .7rem;
}
.fs-0-6{
  font-size: .6rem;
}
.fs-0-5{
  font-size: .5rem;
}
.fs-1{
  font-size: 1rem;
}
.fs-1-1 {
  font-size: 1.1rem;
}
.fs-1-2{
  font-size: 1.2rem;
}
.fs-1-3{
  font-size: 1.3rem;
}
.fs-1-4{
  font-size: 1.4rem;
}
.fs-3{
  font-size: 3rem;
}

</style>
