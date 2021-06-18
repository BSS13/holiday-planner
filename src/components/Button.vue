<template>
 <div>
  <button>
      {{ buttonText }}
  </button>
 </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Button',
  props: {
    buttonText:{
      type: String,
      default: 'Button'
    }
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
div{
   width: 80%;
   margin: auto;
   margin-bottom: 1.5rem;
}
button {
  background-color: #0275d8;
  color: #fff;
  display: block;
  padding: 13px;
  width: 105%;
  border-radius: 4px;
  cursor: pointer;
  border: 1px solid black;
}
button:hover {
    background-color: #f8f9fa;
    color: black;
}
</style>
