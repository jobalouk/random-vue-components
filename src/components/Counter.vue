<template>
  <div>
    {{ count }}
    <a class="button is-danger" @click.prevent="incrementCounter">Count Up</a>
  </div>
</template>

<script>

  export default {
    name: "Counter",
    props: {
      count: Number,
    },
    methods: {
      incrementCounter: function() {
        this.count += 1
      }
    }
  }

</script>
