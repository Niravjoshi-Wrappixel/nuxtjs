<template>
  <div>
    <!-- -----------------------------------------
  Banner
  ----------------------------------------- -->
    <Banner />
    <GrowLearn />
    <Featured />
    <SeoFeatureCards />
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Index Page",
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
    Banner: () => import("@/components/sections/Banner"),
    GrowLearn: () => import("@/components/sections/GrowLearn"),
    Featured: () => import("@/components/sections/Featured"),
    SeoFeatureCards: () => import("@/components/sections/SeoFeatureCards"),
  },
};
</script>
