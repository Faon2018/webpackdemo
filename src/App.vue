<template>
  <div id="app">
    <Head  :title="title">
      <div slot="left"></div>
    </Head>
    <router-view></router-view>
  </div>
</template>

<script>
import Head from './components/common/Head'
export default {
  name: 'App',
  data(){
    return {
        title:''
    }
  },
  components:{
      Head
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
</style>
