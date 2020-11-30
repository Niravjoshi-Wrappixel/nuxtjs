<template>
  <div>
    <!-- -----------------------------------------------
        Start Banner Cards
    ----------------------------------------------- -->
    <v-row class="banner-card-spacer">
      <v-col cols="12" sm="6" md="6" lg="3">
        <v-card class="card-hover2 banner-card">
          <v-card-text class="banner-card-content pb-0">
            <img src="/img/feature1.png" alt="identification" />
            <h4 class="font-weight-bold banner-card-title mt-3">
              Identification
            </h4>
            <p class="banner-card-subtext">
              Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </v-card-text>
          <div class="banner-card-footer pt-0">
            <v-btn text color="primary" class="px-0 font-weight-semibold">
              Learn More
            </v-btn>
          </div>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="3">
        <v-card class="card-hover2 banner-card top-spacer">
          <v-card-text class="banner-card-content pb-0">
            <img src="/img/feature2.png" alt="identification" />
            <h4 class="font-weight-bold banner-card-title mt-3">
              Technical Seo
            </h4>
            <p class="banner-card-subtext">
              Quis ipsum suspendisse ultrices gravida. Risus commodo viverr.
            </p>
          </v-card-text>
          <div class="banner-card-footer pt-0">
            <v-btn text color="primary" class="px-0 font-weight-semibold">
              Learn More
            </v-btn>
          </div>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="3">
        <v-card class="card-hover2 banner-card">
          <v-card-text class="banner-card-content pb-0">
            <img src="/img/feature3.png" alt="identification" />
            <h4 class="font-weight-bold banner-card-title mt-3">On Page Seo</h4>
            <p class="banner-card-subtext">
              Risus commodo viverra maecenas accumsan lacus vel facilisis.
            </p>
          </v-card-text>
          <div class="banner-card-footer pt-0">
            <v-btn text color="primary" class="px-0 font-weight-semibold">
              Learn More
            </v-btn>
          </div>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="3">
        <v-card class="card-hover2 banner-card top-spacer">
          <v-card-text class="banner-card-content pb-0">
            <img src="/img/feature4.png" alt="identification" />
            <h4 class="font-weight-bold banner-card-title mt-3">
              Off Page Seo
            </h4>
            <p class="banner-card-subtext">
              Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </v-card-text>
          <div class="banner-card-footer pt-0">
            <v-btn text color="primary" class="px-0 font-weight-semibold">
              Learn More
            </v-btn>
          </div>
        </v-card>
      </v-col>
    </v-row>
    <!-- -----------------------------------------------
        End Banner Cards
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "BannerCards",

  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss">
</style>