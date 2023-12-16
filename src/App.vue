<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Menu</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <a class="nav-link active" aria-current="page" href="#">Home</a>
        <a class="nav-link" href="#">Prologue</a>
        <a class="nav-link" href="#">blog</a>
      </div>
    </div>
  </div>
</nav>
<div class="container mt-4">
  <h5>React 개발자의 블로그입니다</h5>
    <p>- Vue로 만들었음</p>
</div>
<List :블로그글="블로그글" />

</template>

<script>
import blog from './assets/blog.js'
import List from './components/List.vue'

export default {
  name: 'App',
  data(){
    return {
      블로그글 : blog
    }
  },
  components: {
    List : List,
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
