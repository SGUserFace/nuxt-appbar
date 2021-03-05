<template>

  <v-navigation-drawer :value="isActive" app fixed temporary/>

</template>

<script>
export default {

  name: 'AppNav',

  props: [
    'isActive',
  ],

}
</script>
