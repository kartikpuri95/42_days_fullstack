<template>
    <div>
      <div v-for="post in posts" :key="post.id">
        <h2><RouterLink :to="'/post/' + post.id">{{ post.title }}</RouterLink></h2>
        <p>{{ post.content }} </p>
        <span>written by </span><b>{{post.author}}</b>
      </div> 
    </div>
  </template>
  
  <script>
  export default {
    props: {
      posts: Array
    }
  }
  </script>
  