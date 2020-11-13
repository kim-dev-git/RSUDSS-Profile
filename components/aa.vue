<template>
  <div
    class="grey lighten-4"
  >
    <p v-text="post.title" />
    <span v-text="post.content" />
  </div>
</template>

<script>
export default {
  data: () => ({
    post: {
      title: 'A',
      content: 'asjbdka kjabsdk a'
    }
  })
}
</script>

<style>

</style>