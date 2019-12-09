<template>
  <div id="app">
    {{count}}
    <br>
    <!-- {{$store.getters.doubleCount}} -->
    <br>
    <button @click="$store.commit('increment')">count++</button>
    <!-- <button @click="$store.dispatch('asyncIncrement')">doublecount++</button> -->
  </div>
</template>

<script>

export default {
  name: 'app',
  computed: {
    count() {
      return this.$store.state.count
    }
  }
}
</script>

<style>
</style>
