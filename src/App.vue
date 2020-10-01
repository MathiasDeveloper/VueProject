<template>
  <v-app>
    <Menu></Menu>
    <v-content>
      <router-view />
    </v-content>
  </v-app>
</template>

<script>

import Menu from "./components/Menu";
export default {
  name: 'App',

  components: {
    Menu
  },

  data: () => ({

  }),
};
</script>

<style scoped>

</style>
