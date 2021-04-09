<template>
  <div id="app" class="box-border">
    <div class="container grid">
      <LeftSide />
      <RightSide />
    </div>
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
  
}
.container {
  margin: 0 auto;
  max-width: 1200px;
  grid-template-columns: 63% 1fr;
}
</style>
