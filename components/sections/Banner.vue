<template>
  <div class="banner-wrapper">
    <v-container>
      <!-- -----------------------------------------------
        Start Banner
    ----------------------------------------------- -->
      <!-- Search Section -->
      <BannerSearch />
      <!-- Banner Feature Cards -->
      <BannerCards />
      <!-- -----------------------------------------------
        End Banner
    ----------------------------------------------- -->
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Banner",

  components: {
    BannerSearch: () => import("@/components/sections/BannerSearch"),
    BannerCards: () => import("@/components/sections/BannerCards"),
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss">
</style>