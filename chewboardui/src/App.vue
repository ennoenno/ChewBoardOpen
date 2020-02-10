<template>
  <div id="app">
    <h1 class="header">ChewBoard</h1>
        <Comments v-bind:comments="comments"/>
  </div>
</template>

<script>
import Comments from './components/Comments'

export default {
  name: 'App',
  components: {
      Comments
  },
  data() {
    return {
      comments: [
        {
        id: 1,
        title: 'Erster Kommentar',
        owner: 'Enno'
      },
      {
        id: 2,
        title: 'zweiter Kommentar',
        owner: 'Bumi'
      },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.header {
  padding: 10px;
  background-color: #798c9e;
  margin: 0px;
}
body {
  margin: 0px;
}
</style>
