<template>
  <v-app-bar
    fixed
    dark
    flat
    :color="onTop ? 'transparent' : 'success'"
  >
    <v-container>
      <v-layout
        class="align-center"
      >
        <v-toolbar-title v-text="'RSUDSS'" />
        <v-spacer />
        <v-btn
          color="primary"
        >
          Hallo
        </v-btn>
      </v-layout>
    </v-container>
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({
    onTop: true
  }),
  methods: {
    changeColor() {
      if (
        document.body.scrollTop > 100 ||
        document.documentElement.scrollTop > 100
      ) {
        this.onTop = false
      } else {
        this.onTop = true
      }
    }
  },
  beforeMount () {
    window.onscroll = () => {
      this.changeColor()
    }
  }
}
</script>

<style>

</style>