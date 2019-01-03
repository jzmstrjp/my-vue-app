<template>
  <div>
    <h1 class="title">My Blog App</h1>
    <ul class="posts">
        <li v-for="(post,key) in posts" :key="key">
          <figure class="single_post">
            <figcaption class="single_post__fig_caption">
              <p class="single_post__title">{{post.title}}</p>
              <p class="single_post__body">{{post.body}}</p>
            </figcaption>
            <div class="single_post__img">
              <img src="~/assets/images/color-the-tag-name.png">
            </div>
          </figure>
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
      posts: [
        {
          "title": "タグに色つけ太郎",
          "body": "最初の記事です。",
          "genre": "プラグイン",
          "img": "color-the-tag-name.png",
        },
      ],
    }
  }  
}
</script>
