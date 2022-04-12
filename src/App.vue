<template>
  <div id="app">
   
    <header>
      <LogoComponent/>
      <HeaderNavComponent/>
    </header>
    
  </div>
</template>

<script>
import LogoComponent from './components/LogoComponent.vue'
import HeaderNavComponent from './components/HeaderNavComponent.vue'

export default {
  name: 'App',
  components: {
   LogoComponent,
   HeaderNavComponent,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  max-width: 1440px;
  width: 80%;
  margin: 0 auto;
}

header{
  display: flex;
  justify-content: center;
  justify-content: space-between;
  align-items: center;
  background-color: white;
}
</style>
