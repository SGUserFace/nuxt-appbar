<template>

    <v-app-bar fixed app>
      <v-app-bar-nav-icon @click.stop="changeDrawer"/>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
    </v-app-bar>

</template>

<script>
export default {

  name: 'AppBar',

  props: {
    title: {
      type: String,
      required: false,
    },
  },

  methods: {
    changeDrawer() {
      this.$emit('drawer');
    },
  },

}
</script>
