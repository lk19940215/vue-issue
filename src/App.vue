<template>
  <div id="app">
    <div v-for="i in 2">
      <div @click="functionClickHandle(i)">{{i}}</div>
    </div>
    <div v-for="i in 2">
      <div @click="itemClick(i)">{{i}}</div>
    </div>
  </div>
  <!-- <p></p> -->
</template>

<script>

export default {
  methods: {
    functionClickHandle(res) {
      window.alert( res + 'i am big boss')
      console.log( res + 'i am big boss')
    },
    itemClick() {
      window.alert('item click changed')
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app > div {
  padding: 10px 0;
}
</style>
