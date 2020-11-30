<template>
  <div>
    <!-- -----------------------------------------------
          Start Header
    ----------------------------------------------- -->
    <v-app-bar
      app
      fixed
      class="app-header"
      color="white"
      flat
      elevate-on-scroll
    >
      <v-container class="py-0 fill-height">
        <!-- Logo -->
        <Logo />
        <v-spacer></v-spacer>
        <!-- Desktop view Navigation -->
        <Navigation class="d-none d-lg-flex" />
        <v-spacer></v-spacer>
        <v-btn
          class="d-none d-lg-flex btn-hover"
          color="primary"
          nuxt
          to="/inspire"
          elevation="0"
        >
          Login - Register
        </v-btn>
        <!-- Mobile Hamburger button -->
        <div class="d-block d-lg-none">
          <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
        </div>
      </v-container>
    </v-app-bar>
    <!-- -----------------------------------------------
          End Header
    ----------------------------------------------- -->

    <!-- -----------------------------------------------
          Start Mobile Navigation
    ----------------------------------------------- -->
    <v-navigation-drawer v-model="drawer" absolute temporary>
      <div class="pa-4 d-flex align-items-center">
        <!-- Logo -->
        <Logo />
        <div class="ml-auto">
          <!-- Close button -->
          <v-btn
            @click.stop="drawer = !drawer"
            small
            elevation="0"
            class="white"
          >
            <v-icon>mdi-window-close</v-icon>
          </v-btn>
        </div>
      </div>
      <MobileNavigation />
    </v-navigation-drawer>
    <!-- -----------------------------------------------
          End Mobile Navigation
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "Header",

  components: {
    Logo: () => import("@/components/Logo"),
    Navigation: () => import("@/components/Navigation"),
    MobileNavigation: () => import("@/components/MobileNavigation"),
  },
  data() {
    return {
      drawer: null,
    };
  },
  methods: {},
};
</script>

<style lang="scss">
</style>