<template>
  <div class="character text-center">
      <img :src="info.image" :alt="info.name">
      <h3>{{info.name}}</h3>
      <hr>
      <div>{{info.origin}}</div>
      <div><strong>{{info.type}}</strong></div>
  </div>
</template>

<script>
export default {
    name: "Card",
    props: ['info']
}
</script>

<style lang="scss" scoped>
  img{
    border-radius: 50%;
    max-width: 100%;
  }

  hr{
    width: 50px;
    margin-left: auto;
    margin-right: auto;
    opacity: 1;
  }
</style>