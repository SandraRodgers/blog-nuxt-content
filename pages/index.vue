<template>
  <div>
    <filter-bar></filter-bar>
    <div class="container mx-auto">
      <div class="posts">
        <Card
          v-for="post in posts"
          :key="post.path"
          :v-if="posts"
          :post="post"
        />
      </div>
    </div>
  </div>
</template>

<script>
import FilterBar from '~/components/FilterBar.vue'
export default {
  components: { FilterBar },
  layout: 'home',
  async asyncData({ $content }) {
    const posts = await $content('blog')
      .only(['path', 'title', 'cover', 'date', 'readingTime', 'slug', 'dir'])
      .where({ date: { $lt: Date.now() } })
      .sortBy('date', 'desc')
      .limit(3)
      .fetch()
    return {
      posts,
    }
  },
}
</script>

<style>
.container {
  margin: 0 auto;
  /* min-height: 50vh; */
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.posts {
  display: flex;
}
</style>
