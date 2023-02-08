<template>
  <v-app class="overflow-hidden">
    <v-app-bar
      absolute
      app
      color="orange darken-3"
      dark
      :collapse="!collapseOnScroll"
      :collapse-on-scroll="collapseOnScroll"
      scroll-target="#scrolling-techniques-6"
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          :src="logo"
          transition="scale-transition"
          width="40"
        />

<!--        <v-img-->
<!--          alt="Vuetify Name"-->
<!--          class="shrink mt-1 hidden-sm-and-down"-->
<!--          contain-->
<!--          min-width="100"-->
<!--          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"-->
<!--          width="100"-->
<!--        />-->
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href=""
        text
        depressed
      >
        <span class="mt-1">
        <v-icon class="mr-2 mb-2">mdi-file-document</v-icon>
          Resume</span>
      </v-btn>
    </v-app-bar>

    <v-sheet
        id="scrolling-techniques-6"
        class="overflow-y-auto"
        max-height="2000"
    >

    <v-main>
      <router-view/>
    </v-main>
    </v-sheet>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
    logo: require('@/assets/05.svg'),
    collapseOnScroll: true,
  }),
};
</script>

<style>
v-btn {
  border-radius: 20px;
}
</style>