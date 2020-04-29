<template>
  <div class="blogs">
    <h2>Blogs</h2>
    <ul>
      <li v-for="blog in blogs" :key="blog.id">
        <b-button>{{ blog.name }}</b-button>
        <hr />
      </li>
    </ul>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      blogs: [
        {
          id: 1,
          name: 'Intro VueJS'
        },
        {
          id: 2,
          name: 'Intro NuxtJS'
        },
        {
          id: 3,
          name: 'Advan NuxtJS'
        }
      ]
    }
  }
}
</script>

<style></style>
