<template>
  <v-bottom-nav
    :active.sync="bottomNav"
    :value="true"
    absolute
    app
    color="transparent"
  >
    <v-btn
      color="secondary"
      flat
      value="recent"
    >
      <span>Зона 1</span>
      <v-icon>history</v-icon>
    </v-btn>

    <v-btn
      color="secondary"
      flat
      :to="{name: 'Profile'}"
      value="favorites"
    >
      <span>Зона 2</span>
      <v-icon>favorite</v-icon>
    </v-btn>

    <v-btn
      color="secondary"
      flat
      value="nearby"
    >
      <span>Зона 3</span>
      <v-icon>place</v-icon>
    </v-btn>
  </v-bottom-nav></template>
<style>
  .main-sidebar .list__group__items--no-action .list__tile {
    padding-left: 36px !important;
  }
</style>
<script type="text/babel">
  export default {
    name: 'BottomNav',
    data () {
      return {
        bottomNav: 'recent'
      }
    }
  }
</script>

