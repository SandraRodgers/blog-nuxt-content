<template>
  <div class="card">
    <nuxt-link :to="`/blog/${post.slug}/`" :title="post.title">
      <h1 class="post-title">{{ post.title }}</h1>
      <hr />
      <p>{{ eventDate(post.date) }}</p>
    </nuxt-link>
  </div>
</template>

<script>
import moment from 'moment'
export default {
  props: ['post'],
  methods: {
    eventDate(date) {
      return moment(date).format('MMMM DD, YYYY')
    },
  },
}
</script>

<style scoped>
.card {
  align-items: center;
  border: rgb(220, 223, 223) solid 1px;
  border-radius: 1px;
  color: rgb(41, 44, 44);
  display: flex;
  font-family: 'Montserrat';
  height: 60vh;
  justify-content: center;
  padding: 20px;
  width: 33vw;
}

.post-title {
  font-size: 2em;
}

a {
  color: rgb(41, 44, 44);
  text-decoration: none;
}

hr {
  width: 80px;
  height: 1px;
  border: 0;
  margin: 15px auto;
  display: block;
  background-color: #bbb;
}
</style>