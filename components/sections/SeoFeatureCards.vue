<template>
  <div class="featurecard-wrapper">
    <!-- -----------------------------------------------
        Start Feature Cards
    ----------------------------------------------- -->
    <v-container>
      <h2 class="font-weight-bold text-center section-title">
        We are seo community, that helps you to grow & learn
      </h2>
      <p class="text-center mt-4">
        Lorem ipsum dolor sit amet, sed do eiusmod tempor incididunt
      </p>
      <v-row class="seo-feature-card-top-spacer">
        <v-col
          cols="12"
          lg="6"
          md="6"
          v-for="(item, i) in seofeatureditem"
          :key="i"
        >
          <v-card class="seo-feature-card">
            <v-card-text>
              <v-btn
                fab
                icon
                large
                :color="item.icontextcolor"
                :class="item.iconbgcolor"
                class="elevation-0 seo-feature-icon"
              >
                <i :class="item.icon"></i>
              </v-btn>
              <h4 class="text-h4">{{ item.title }}</h4>
              <p class="seo-feature-subtext">
                {{ item.subtext }}
              </p>
              <v-btn text color="primary" class="px-0 font-weight-semibold">
                Learn More
              </v-btn>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <!-- -----------------------------------------------
        End Feature Cards
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "SeoFeatureCards",

  components: {},
  data: () => ({
    seofeatureditem: [
      {
        icontextcolor: "primary",
        iconbgcolor: "primary-lighten-5",
        icon: "fas fa-question",
        title: "Questions",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        icontextcolor: "error",
        iconbgcolor: "error-lighten-5",
        icon: "fas fa-cloud-download-alt",
        title: "Resources",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        icontextcolor: "success",
        iconbgcolor: "success-lighten-5",
        icon: "fas fa-play",
        title: "Videos",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        icontextcolor: "info",
        iconbgcolor: "info-lighten-5",
        icon: "fas fa-wrench",
        title: "Tools",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        icontextcolor: "warning",
        iconbgcolor: "warning-lighten-5",
        icon: "fas fa-leaf",
        title: "Articles",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
      {
        icontextcolor: "accent",
        iconbgcolor: "accent-lighten-5",
        icon: "fas fa-tag",
        title: "Topics",
        subtext:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      },
    ],
  }),
  methods: {},
};
</script>

<style lang="scss">
</style>