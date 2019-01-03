<template>
  <div class="single_post_page">
    <h1 class="title">{{post.title}}</h1>
    <figure class="single_post_fig">
      <figcaption class="single_post_fig__caption">
        <p class="single_post__body">{{post.body}}</p>
        <div class="single_post_link">
          <a v-bind:href="post.url" target="_blank">{{post.link_text}}を見る</a>
        </div>
      </figcaption>
      <div v-if="post.img" class="single_post_fig__img">
        <img v-bind:src="require('~/assets/images/' + post.img)">
      </div>
    </figure>
    <div class="back_to_top">
      <router-link to="/">Back</router-link>
    </div>    
  </div>
</template>

<script>
import Posts from '~/components/posts.vue'
export default {
  data(){
    return {
      post: Posts[this.$route.params.id],
    }
  }  
}
</script>