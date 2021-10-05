<template>
  <div id="app">
    <Header title="Rick and Morty App"/>
    <main>
    <Characters/>
    </main>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Characters from './components/Characters.vue'

export default {
  name: 'App',
  components: {
    Header,
    Characters,
  },
  data(){
    return {

    }
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common";

</style>
