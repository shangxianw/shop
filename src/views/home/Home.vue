<template>
  <div>
    <GoodsCard />
  </div>
</template>

<script>
import GoodsCard from "./components/GoodsCard.vue"
export default {
  components: { GoodsCard },
  data() {
    return {

    }
  },

  setup() {
    function tabSwitch(item, index) {
      console.log(item, index);
    }
    return {
      tabSwitch,
    };
  },
}
</script>

<style scoped>
.card {
  width: 360px;
  height: 360px;
  margin: 0 auto;
}
</style>