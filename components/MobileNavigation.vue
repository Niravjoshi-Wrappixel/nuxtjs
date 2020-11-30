<template>
  <div class="pa-4">
    <!-- -----------------------------------------------
          Start Listing of item (Navigation)
    ----------------------------------------------- -->
    <v-list dense>
      <v-list-item-group
        v-model="group"
        active-class="primary--text text--accent-4"
      >
        <v-list-item
          v-for="link in data"
          :key="link.id"
          link
          nuxt
          :to="link.to"
        >
          <!-- <v-list-item-icon>
            <v-icon>{{ link.icon }}</v-icon>
          </v-list-item-icon> -->

          <v-list-item-content>
            <v-list-item-title>{{ link.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
    <!-- -----------------------------------------------
          End Listing of item (Navigation)
    ----------------------------------------------- -->

    <v-btn color="primary" block nuxt to="/inspire" elevation="0">
      Login - Register
    </v-btn>
  </div>
</template>

<script>
import data from "../data/navigation.json";

export default {
  name: "MobileNavigation",
  components: {
    Logo: () => import("@/components/Logo"),
  },
  data() {
    return {
      data,
      group: null,
    };
  },
  methods: {},
};
</script>
<style lang="scss">
</style>