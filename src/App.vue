<template>
  <div class="home">
    <h1>Home</h1>
    <PostList :posts="posts" />
  </div>
</template>

<script>
import PostList from './components/PostList.vue'
import { ref } from "vue";

export default {
  name: "Home",
  components: { PostList },
  setup() {
    const posts = ref([
      {title: 'welcome to the blog', body: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus hic nobis quos dolor maxime nihil asperiores modi omnis error tempore. Corporis consequuntur ratione ducimus earum?', id: 1 },
      {title: 'top 5 css tips', body: 'lorem impsum', id: 2 }
    ])

    return { posts };
  },
};
</script>

