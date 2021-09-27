<template>
  <div>
    <SearchJokes v-on:search-text="searchText" />
    <Joke v-for="joke in jokes" :key="joke.id" :id="joke.id" :joke="joke.joke" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Joke from '../../components/Joke'
import SearchJokes from '../../components/SearchJokes.vue'

export default Vue.extend({
  components: {
    Joke,
    SearchJokes
  },
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
      const res = await this.$axios.get('https://icanhazdadjoke.com/search?term=dad', config);
      this.jokes = res.data.results;
    } catch(err) {
      console.log(err);
    }
  },
  methods: {
    async searchText(text) {
      const config = {
        headers: {
          'Accept': 'application/json'
        }
      }
      try {
        const res = await this.$axios.get(`https://icanhazdadjoke.com/search?term=${text}`, config);
        this.jokes = res.data.results;
      } catch(err) {
        console.log(err);
      }
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
