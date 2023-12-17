<template>
<div v-for="(a, i) in 블로그글" :key="i">
  <ol class="list-group">
  <li class="list-group-item d-flex justify-content-between align-items-start">
    <div class="ms-1 me-auto">
      <div @click="$router.push('/detail/' + i)" class="fw-bold">{{i+1}}. {{ 블로그글[i].title}}</div>
      {{ 블로그글[i].date }}
    </div>
    <span class="badge bg-primary rounded-pill">{{ 블로그글[i].number }}</span>
  </li>
</ol>

</div>
</template>

<script>
export default {
    name: 'list',
    props : {
    블로그글 : Array
}

}


</script>

<style>

</style>