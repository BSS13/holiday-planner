<template>
  <header>
    <h1>{{ headerTitle }}</h1>
  </header> 
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Header',
  props: {
    headerTitle:{
      type: String,
      default: 'Holiday Planner'
    }
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1 {
  margin: auto;
  text-align: center;
}
</style>
