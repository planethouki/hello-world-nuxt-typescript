<template lang="pug">
  .container
    div
      logo
      h1.title
        | nuxt-ts-example
      h2.subtitle
        | My beautiful Nuxt.js project
      .links
        a.button--green(href="https://nuxtjs.org/" target="_blank") Documentation
        a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank") GitHub
</template>

<script lang="ts">
import Logo from '~/components/Logo.vue'
import Vue, { PropOptions } from 'vue'

export default Vue.extend({
    components: { logo: Logo },
    data () {
        return {
            message: 'This is a message'
        }
    }
})
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
