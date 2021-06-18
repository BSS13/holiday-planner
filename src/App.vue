<template>
  <Header headerTitle="Holiday Planner"/>
  <Input labelText="How long is your vacation?" placeholderText="Number of days"/>
  <Button buttonText="Calculate Best Dates"/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Header from './components/Header.vue';
import Button from './components/Button.vue';
import Input from './components/Input.vue';

export default defineComponent({
  name: 'App',
  components: {
    Header,
    Button,
    Input
  }
});
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto+Condensed');
*{
  background-color: #FAFAFA;
}
#app {
  font-family:  'Roboto' ,Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 16px;
  margin-top: 60px;
}
</style>
