<template>

  <v-app>
    <app-bar @drawer="changeDrawer" />
    <app-nav :isActive="drawer" />
  </v-app>

</template>

<script>
export default {
  data() {
    return {
      drawer: false,
    }
  },

  methods: {
    changeDrawer() {
      this.drawer = !this.drawer;
    },
  },

}
</script>
