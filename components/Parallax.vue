<template>
  <v-parallax
    dark
    :src="img"
  >
    <v-row
      align="center"
      justify="center"
      class="mx-n4"
      style="background-color: rgba(0, 0, 0, .5)"
    >
      <v-col
        class="text-center"
        cols="12"
      >
        <h1 class="display-1 font-weight-bold mb-4" v-text="title || ''" />
        <h4 class="subheading font-weight-thin" v-text="caption || ''" />
        <v-layout
          column
          class="align-center mt-4"
        >
          <v-sheet
            height="4px"
            width="120px"
            color="success"
            rounded
          />
        </v-layout>
      </v-col>
    </v-row>
  </v-parallax>
</template>

<script>
export default {
  props: [
    'img',
    'title',
    'caption',
  ]
}
</script>

<style>

</style>