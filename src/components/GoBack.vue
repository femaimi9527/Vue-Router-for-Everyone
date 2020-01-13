<template>
  <span class="go-back">
    <button @click="goBack">Go Back</button>
  </span>
</template>

<script>
export default {
  methods: {
    goBack() {
      return this.$router.go(-1);
    }
  }
};
</script>

<style scoped>
.go-back {
  display: flex;
  cursor: pointer;
}
button {
  border: 0;
  font-size: 15px;
  font-weight: bold;
  border-radius: 3px;
  background: rgba(0, 0, 0, 0.2);
}
</style>
