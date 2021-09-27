<template>
  <div>
    <h1>About Dad Jokes</h1>
    <p>This is an app that displays corny Dad Jokes.</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'About The App',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Best place for corny dad joked'
        }
      ]
    }
  }
})
</script>
