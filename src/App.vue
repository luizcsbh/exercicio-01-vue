<template>
  <div id="app">
    <div id="header">
      <img alt="Vue logo" src="./assets/logo.png">
      <Header/>
    </div>
    <div id="body">
      <Menu/>
      <div>
        <Sidebar />
        <Article/>
        
      </div>
      
    </div>
  </div>
</template>

<script>
import Article from './components/Article.vue'
import Header from './components/Header.vue'
import Menu from './components/Menu.vue'
import Sidebar from './components/Sidebar.vue'

export default {
  name: 'App',
  components: {
    Article,
    Header,
    Menu,
    Sidebar
  }
}
</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#header {
  text-align: left;
}

#body{
  border:1px solid;
  width: 100%;
  
}
</style>
