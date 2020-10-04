<template>
  <div id="app">
    <Counter v-bind:count="0" />
    <Form />
  </div>
</template>

<script>
import Counter from './components/Counter.vue'
import Form from './components/Form.vue'


export default {
  name: 'App',
  components: {
    Counter,
    Form,
  }
}
</script>

<style>

</style>
