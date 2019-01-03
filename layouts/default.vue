<template>
  <div>
    <header>
      <div class="inner">
        <div class="site_name">
          <span class="ib">Takashi Tokumoto</span>
          <span class="ib">Portfolio Website</span>
        </div>
      </div>
    </header>
    <main>
      <div class="inner">
        <nuxt/>
      </div>
    </main>
    <footer>
      <div class="inner">
        <div class="copyright">
          <small>&copy;&nbsp;2019&nbsp;jzmstrjp</small>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Concert+One');
html {
  font-family: 'Concert One', "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 10px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  font-size: 1.6rem;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

img {
  max-width: 100%;
}

a {
  text-decoration: none;
  color: inherit;
}

.inner {
  width: 1200px;
  max-width: 90%;
  margin-left: auto;
  margin-right: auto;
}

header, footer {
  text-align: center;
}

header {
  margin-bottom: 2rem;
}

footer {
  margin-top: 2rem;
}

.site_name {
  font-size: 3rem;
  padding: 1rem;
}

.back_to_top {
  text-align: center;
  margin-top: 3rem;
  a{
    border: 2px solid;
    font-weight: bold;
    display: inline-block;
    padding: 0.5em 1em;
    border-radius: 0.5em;
  }
}

.title {
  margin-bottom: 2rem;
}

.single_post_fig__img {
  margin-top: 2rem;
}

.copyright {
  padding: 0.7em 0 0.8em;
}

.page-enter-active, .page-leave-active {
  transition: .5s;
}
.page-enter, .page-leave-to {
  opacity: 0;
}
.page-enter {
  transform: translateX(100%);
}
.page-leave-to {
  transform: translateX(-100%);
}
</style>

