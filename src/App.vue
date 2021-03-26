<template>
  <div id="app">
    <Sidebar/>
    <div class="wrapper">
      <p>Приветbr мир</p>

    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar'

export default {
  name: 'App',
  components: {
    Sidebar
  }
}
</script>

<style lang="scss">
#app {
  width:100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  /*font-family: Avenir, Helvetica, Arial, sans-serif;*/
  /*-webkit-font-smoothing: antialiased;*/
  /*-moz-osx-font-smoothing: grayscale;*/
  /*text-align: center;*/
  /*color: #2c3e50;*/
  /*margin-top: 60px;*/
}

  .wrapper{
    height:2000px;

  }
</style>
