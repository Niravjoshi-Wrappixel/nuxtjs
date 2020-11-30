<template>
  <div>
    <!-- -----------------------------------------------
        Start Banner Search
    ----------------------------------------------- -->
    <v-row justify="center">
      <v-col cols="12" sm="10" md="8">
        <h1 class="banner-title font-weight-bold text-center">
          Welcome to the SEODebate Community
        </h1>
        <div>
          <v-text-field
            class="search-widget"
            placeholder="Search anything"
            hide-details="auto"
          >
            <v-icon slot="prepend" class="fas fa-search"> </v-icon>
          </v-text-field>
        </div>
      </v-col>
    </v-row>
    <!-- -----------------------------------------------
        End Banner Search
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "BannerSearch",

  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss">
</style>