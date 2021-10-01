<template>
  <div id="app">
    <Header title="Rick and Mortty app"/>
    <main>
    <Searchbar/>
    <Characters/>
    </main>
  </div>
</template>

<script>
import Searchbar from './components/Searchbar.vue'
import Header from './components/Header.vue'
import Characters from './components/Characters.vue'

export default {
  name: 'App',
  components: {
    Header,
    Searchbar,
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
