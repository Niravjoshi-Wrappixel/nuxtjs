<template>
  <div class="container growlearn-wrapper">
    <!-- -----------------------------------------------
        Start GrowLearn
    ----------------------------------------------- -->
    <h2 class="font-weight-bold text-center section-title">
      We are seo community, that helps you to grow & learn
    </h2>
    <p class="text-center mt-4">
      Lorem ipsum dolor sit amet, sed do eiusmod tempor incididunt
    </p>

    <!-- Cards -->
    <v-row class="grow-card-row" justify="center">
      <v-col cols="12" sm="6" md="6" lg="4">
        <v-card class="elevation-0 grow-card">
          <v-card-text class="px-0">
            <div class="d-md-flex align-start">
              <v-btn depressed color="primary" class="grow-icon">
                <img src="/img/grow1.png" alt="" />
              </v-btn>
              <div class="grow-card-content">
                <h2 class="font-weight-bold primary--text mt-3">
                  Free Support
                </h2>
                <p class="subtext-spacer">
                  Consectetur adipiscing elit, sed do eiusmod tempor incididunt
                  ut labore et dolore magna aliqua.
                </p>
              </div>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="4">
        <v-card class="elevation-0 grow-card">
          <v-card-text class="px-0">
            <div class="d-md-flex align-start">
              <v-btn depressed color="primary" class="grow-icon">
                <img src="/img/grow2.png" alt="" />
              </v-btn>
              <div class="grow-card-content">
                <h2 class="font-weight-bold primary--text mt-3">
                  SEO Magicians
                </h2>
                <p class="subtext-spacer">
                  Sed do eiusmod tempor incididunt ut labore et dolore magna
                  aliqua. Quis ipsum suspendisse ultrices gravida.
                </p>
              </div>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6" lg="4">
        <v-card class="elevation-0 grow-card">
          <v-card-text class="px-0">
            <div class="d-md-flex align-start">
              <v-btn depressed color="primary" class="grow-icon">
                <img src="/img/grow3.png" alt="" />
              </v-btn>
              <div class="grow-card-content">
                <h2 class="font-weight-bold primary--text mt-3">Resources</h2>
                <p class="subtext-spacer">
                  Quis ipsum suspendisse ultrices gravida. Risus commodo viverra
                  maecenas accumsan lacus vel facilisis.
                </p>
              </div>
            </div>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <GrowLearnVideo />
    <!-- -----------------------------------------------
        End GrowLearn
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "GrowLearn",

  components: {
    GrowLearnVideo: () => import("@/components/sections/GrowLearnVideo"),
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss">
</style>