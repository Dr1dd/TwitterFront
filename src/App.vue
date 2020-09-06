<template>
  <div id="app">
    <Header />
    <Tweets />
    <Search />
  </div>
</template>

<script>
import Header from './components/Header'
import Tweets from './components/MainContent'
import Search from './components/Search'
export default {
  name: 'App',
  components: {
    Header,
    Tweets,
    Search
  }
}
</script>

<style lang="scss">
:root{
  --base-color: rgb(21, 32, 43);
  --tweet-content-width-l: 600px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
  width: 100%;
  display: flex;
  flex-direction: row;
  
}
body{
  margin: 0px;
  background-color: var(--base-color);
}
</style>
