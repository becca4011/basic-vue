<template>
  <div>
    <p>{{ name }}</p>
    <br />
    <button @click="updateName">Change Name</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "Becca",
    };
  },
  methods: {
    updateName() {
      this.name = "Becca Updated";
    },
  },
};
</script>

<style scoped>
</style>