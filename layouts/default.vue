<template>
  <v-app dark>
    <Header />
    <v-main>
      <nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
export default {
  head() {
    return {
      title: "SEO Debate - The Vuetify Template",
      meta: [
        {
          hid: "description",
          name: "SEO Debate",
          content: "SEO Debate is the best way",
        },
      ],
    };
  },
  components: {
    Header: () => import("@/components/Header"),
    Footer: () => import("@/components/Footer"),
  },
};
</script>

<style>
</style>
