<template>
  <!-- -----------------------------------------------
        Start Desktop Navigation item
  ----------------------------------------------- -->
  <div class="navigation">
    <ul class="navbar-nav">
      <li class="nav-item" v-for="link in data" :key="link.id" text>
        <n-link class="nav-link" nuxt :to="link.to">
          {{ link.title }}
        </n-link>
      </li>
    </ul>
  </div>
  <!-- -----------------------------------------------
        End Desktop Navigation item
  ----------------------------------------------- -->
</template>

<script>
import data from "../data/navigation.json";
export default {
  name: "Navigation",
  data() {
    return {
      data,
    };
  },
};
</script>

<style lang="scss">
</style>