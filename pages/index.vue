<template>
  <div>
    <h1 class="title">My Blog App</h1>
    <ul class="posts_list">
      <li v-for="(post,key) in posts" :key="key">
        <router-link :to="{ name: 'posts-id', params: { id: key }}">
          <figure class="single_post_fig">
            <figcaption class="single_post_fig__caption">
              <p class="single_post__title">{{post.title}}</p>
              <p class="single_post__body">{{post.body}}</p>
            </figcaption>
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
