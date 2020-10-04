<template>
  <div>
    <h1>Vue.js Form Processing</h1>
    <div>

      <form id="signup-form" @submit.prevent="processForm">
        <div class="field">
          <label class="label">Name</label>
          <input
            type="text"
            class="input"
            name="name"
            v-model="name"
          >
        </div>

        <div class="field">
          <label class="label">Email</label>
          <input
            type="email"
            class="input"
            name="email"
            v-model="email"
          >
        </div>
        <button type="submit" class="button is-danger">Submit</button>
      </form>

    </div>
  </div>
</template>


<script>
  export default {
    name: "Form",
    data: function() {
      return {
        name: '',
        email: ','
      }
    },
    methods: {
      processForm: function() {
        console.log(this.name)
      }
    }
  }
</script>
