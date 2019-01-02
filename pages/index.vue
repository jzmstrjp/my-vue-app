<template>
  <div>
    <h1 class="title">My Blog App</h1>
    <ul>
        <li v-for="post in posts" :key="post.id">
          {{post.title}}
        </li>
    </ul>
    <router-link to="/about">トップページへ戻る</router-link>
  </div>
  
</template>

<script>
export default {
  data(){
    return {
      posts: [
        {
          "id": 1,
          "title": "最初の記事です。"
        },
        {
          "id": 2,
          "title": "2番目の投稿です。",
        },
        {
          "id": 3,
          "title": "３番めの投稿です。",
        },
      ]      
    }
  }  
}
</script>
