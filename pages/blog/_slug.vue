<template>
  <div><nuxt-content :document="post" /></div>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    // fetch our post here
    console.log(params)
    const post = await $content('blog', params.slug).fetch()

    return { post }
  },
}
</script>

<style scoped>
</style>