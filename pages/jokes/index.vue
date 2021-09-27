<template>
  <div>
    <Joke v-for="joke in jokes" :key="joke.id" :id="joke.id" :joke="joke.joke" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Joke from '../../components/Joke'

export default Vue.extend({
  data() {
    return {
      jokes: []
    }
  },
  async created() {
    const config = {
      headers: {
        'Accept': 'application/json'
      }
    }
    try {
      const res = await this.$axios.get('https://icanhazdadjoke.com/search?term=hipster', config);
      this.jokes = res.data.results;
    } catch(err) {
      console.log(err);
    }
  },
  head() {
    return {
      title: 'Dad Jokes',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Jokes list'
        }
      ]
    }
  }
})
</script>
