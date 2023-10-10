<template>
  <div>
    <button @click="navigateToWritePost">Write a Post</button>
    <BlogList :posts="posts" />
  </div>
</template>

<script>
import { ref } from 'vue';
import BlogList from '../components/BlogList.vue';

export default {
  components: { BlogList },
  setup() {
    const posts = ref([
      { id: 1, title: 'First Blog Post', content: 'This is the content of the first blog post', author: 'John Doe' },
      // ... add more posts as required
    ]);

    const navigateToWritePost = () => {
      // logic to navigate to a new page to write a post (to be implemented)
    };

    return { posts, navigateToWritePost };
  }
}
</script>
