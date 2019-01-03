<template>
  <div>
    <h1 class="title">My Blog App</h1>
    <ul class="posts">
      <li v-for="(post,key) in posts" :key="key">
        <router-link v-bind:to="{ name : 'Event', params : { id: key }}">あああ</router-link>
        <router-link to="/posts/">
          <figure class="single_post">
            <figcaption class="single_post__fig_caption">
              <p class="single_post__title">{{post.title}}</p>
              <p class="single_post__body">{{post.body}}</p>
            </figcaption>
            <div v-if="post.img" class="single_post__img">
              <img v-bind:src="require('~/assets/images/' + post.img)">
            </div>
          </figure>
        </router-link>
      </li>
    </ul>
    <router-link to="/about">トップページへ戻る</router-link>
  </div>
  
</template>

<script>
import Posts from '~/components/posts.vue'
export default {
  data(){
    return {
      posts: Posts,
    }
  }  
}
</script>
