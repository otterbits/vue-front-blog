<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Menu</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <router-link to="/"><a class="nav-link active" aria-current="page" href="#">Home</a></router-link>
        <router-link to="/list"><a class="nav-link" href="#">Blog</a></router-link>
        <a class="nav-link" href="#">guest</a>
      </div>
    </div>
  </div>
</nav>

<div class="mt-4">
<router-view :블로그글="블로그글"></router-view>
</div>

</template>

<script>
import blog from './assets/blog.js'


export default {
  name: 'App',
  data(){
    return {
      블로그글 : blog
    }
  },
  components: {
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
}
</style>
