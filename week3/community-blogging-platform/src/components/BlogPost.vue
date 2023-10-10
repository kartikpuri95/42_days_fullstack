<template>
    <div class="blog-post">
      <h2>{{ post.title }}</h2>
      <p>{{ post.content }}</p>
      <footer>
      Posted by {{ post.author }} on {{ post.timestamp | formatDate }}
    </footer>    </div>
  </template>
  
  <script>
  export default {
    props: ['post']
  }
  </script>
  