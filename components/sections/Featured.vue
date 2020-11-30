<template>
  <div class="featured-wrapper">
    <!-- -----------------------------------------------
        Start Featured
    ----------------------------------------------- -->
    <v-container>
      <h4 class="font-weight-bold text-h4">Featured</h4>
      <div class="featured-card">
        <div class="featured-item" v-for="(item, i) in featureditem" :key="i">
          <div class="featured-icon">
            <v-btn fab small :color="item.iconcolor" class="elevation-0">
              <i :class="item.icon"></i>
            </v-btn>
          </div>
          <div class="featured-item-content">
            <a
              href="javascript:void(0)"
              class="item-title font-weight-semibold"
            >
              {{ item.title }}
            </a>
            <div class="d-md-flex align-center mt-3">
              <div class="d-md-flex">
                <span :class="item.badgebg" class="badge">{{
                  item.badgetext
                }}</span>
                <div
                  class="ml-0 ml-md-7 mt-4 mt-md-0 pr-7 border-right border-sm-right-0"
                >
                  <span
                    >In
                    <a href="javascript:void(0)" class="category-title">{{
                      item.categorytitle
                    }}</a></span
                  >
                </div>
              </div>

              <div class="ml-0 ml-md-7 d-flex mt-7 mt-md-0">
                <div class="py-2 py-md-0 pr-7 border-right">
                  <span>{{ item.date }}</span>
                </div>
                <div class="ml-7 py-2 py-md-0">
                  <span>{{ item.views }}</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </v-container>
    <!-- -----------------------------------------------
        End Featured
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "Featured",

  components: {},
  data: () => ({
    featureditem: [
      {
        iconcolor: "primary",
        icon: "fas fa-question",
        title:
          "How to choose the right keyword? Which term is better to rank higher is it long tail or short tail keyword?",
        badgebg: "primary-lighten-5 primary--text",
        badgetext: "Questions",
        categorytitle: "On page seo",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
      {
        iconcolor: "success",
        icon: "fas fa-play",
        title:
          "With Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers, they could easily monitor with Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers, they could easily monitor",
        badgebg: "success-lighten-5 success--text",
        badgetext: "Videos",
        categorytitle: "Identification",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
      {
        iconcolor: "warning",
        icon: "fas fa-leaf",
        title:
          "With Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers",
        badgebg: "warning-lighten-5 warning--text",
        badgetext: "Articles",
        categorytitle: "Technical seo",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
      {
        iconcolor: "error",
        icon: "fas fa-cloud-download-alt",
        title:
          "How to choose the right keyword? Which term is better to rank higher is it long tail or short tail keyword?",
        badgebg: "error-lighten-5 error--text",
        badgetext: "Resources",
        categorytitle: "Technical seo",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
      {
        iconcolor: "info",
        icon: "fas fa-wrench",
        title:
          "With Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers, they could easily monitor with Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers, they could easily monitor",
        badgebg: "info-lighten-5 info--text",
        badgetext: "Tools",
        categorytitle: "Technical seo",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
      {
        iconcolor: "accent",
        icon: "fas fa-tag",
        title:
          "With Google (Chrome) & Bing (IE / Edge) controlling the biggest and most used browsers",
        badgebg: "accent-lighten-5 accent--text",
        badgetext: "Topics",
        categorytitle: "Technical seo",
        date: "Sep 25, 2020",
        views: "25,567 Views",
      },
    ],
  }),
  methods: {},
};
</script>

<style lang="scss">
</style>