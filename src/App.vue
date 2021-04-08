<template>
  <div id="app" class="box-border">
    <LeftSide />
    <RightSide />
  </div>
</template>

<script>
import LeftSide from './components/LeftSide.vue';
import RightSide from './components/RightSide.vue';

export default {
  name: 'App',
  components: {
    LeftSide,
    RightSide
  }
}
</script>

<style>
#app {
  font-family: 'Roboto';
  display: grid;
  grid-template-columns: 63% 1fr;
}
</style>
