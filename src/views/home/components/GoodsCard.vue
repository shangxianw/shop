<template>
  <div class="card" @click="onCardClick">
    card
  </div>
</template>

<script>
export default {

  methods: {
    onCardClick() {
      this.$router.push("detail");
    }
  }
}
</script>

<style scoped>
.card {
  width: 360px;
  height: 360px;
  margin: 0 auto;
  background-color: orange;
  border-radius: 8px;
}
</style>