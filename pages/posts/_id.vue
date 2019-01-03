<template>
  <div>
    <h1 class="title">About this App</h1>

    <figure class="single_post">
      <figcaption class="single_post__fig_caption">
        <p class="single_post__title">{{post.title}}</p>
        <p class="single_post__body">{{post.body}}</p>
      </figcaption>
      <div v-if="post.img" class="single_post__img">
        <img v-bind:src="require('~/assets/images/' + post.img)">
      </div>
    </figure>

    <router-link to="/">トップページへ戻る</router-link>    
  </div>
</template>