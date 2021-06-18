<template>
  <div>
   <label>{{ labelText }}</label>
   <input type="number" :placeholder="placeholderText">
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Input',
  props: {
    labelText:{
      type: String,
      default: 'Label'
    },
    placeholderText:{
      type: String,
      default: 'Placeholder'
    }
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div {
   width: 80%;
   margin: auto;
   margin-top: 4.75rem;
   margin-bottom: 2.5rem;
}
label {
   font-weight: 600;
}
input {
  display: block;
  padding: 13px;
  width: 100%;
  margin: 2.5px;
  border-radius: 4px;
  border: 1px solid #d3d3d3;
}
</style>
