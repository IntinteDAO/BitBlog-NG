<template>
  <div>
    <Navbar />
    <Nuxt class="content" />
    <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Navbar,
    Footer
  }
}
</script>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  display: flex;
}

#__nuxt {
  display: flex;
  flex: 1;
}

#__layout {
  display: flex;
  flex: 1;
}

#__layout > div {
  display: flex;
  flex-direction: column;
  flex: 1;
}

#__layout > div > .content {
  flex: 1;
}

.page-enter-active, .page-leave-active { transition: opacity .1s; }
.page-enter, .page-leave-active { opacity: 0; }
</style>
