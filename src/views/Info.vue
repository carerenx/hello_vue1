<template>
  <div class="info">
    <h1>This is an info page</h1>
    <button type="button" @click="add()">添加</button>
  </div>
</template>
<script>
  import store from '@/store'
  export default {
    name: 'Info',
    methods: {
      add() {
        console.log('add Even from info')
        store.commit('increase')
        alert('alter from info')
      }
    }
  };
</script>
