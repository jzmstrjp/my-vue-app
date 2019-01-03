<template>
  <div>
    <header>
      <div class="inner">
        <div class="site_name">jzmstrjp Portfolio Website</div>
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

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
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

.inner {
  width: 1200px;
  max-width: 90%;
  margin-left: auto;
  margin-right: auto;
}

header, footer {
  text-align: center;
  background-color: #000;
  color: #fff;
}

.copyright {
  padding: 1em;
}

.page-enter-active, .page-leave-active {
  transition: opacity .3s;
}
.page-enter, .page-leave-to {
  opacity: 0;
}

</style>

