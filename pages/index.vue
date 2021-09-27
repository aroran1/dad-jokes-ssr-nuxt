<template>
  <div>
    <h1>Welcome to the best corny dad app on the web</h1>
    <br />
    <div>
      <Tutorial />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'Welcome to the best corny dad app',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Welcome to the best corny dad app'
        }
      ]
    }
  }
})
</script>