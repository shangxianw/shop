<template>
  <div>
    <router-view name="home"></router-view>
    <router-view name="game"></router-view>
    <router-view name="user"></router-view>
    <nut-tabbar @tab-switch="tabSwitch" bottom safeAreaInsetBottom>
      <nut-tabbar-item tab-title="首页" to="home" icon="home">
      </nut-tabbar-item>
      <nut-tabbar-item tab-title="游戏" to="game" icon="category">
      </nut-tabbar-item>
      <nut-tabbar-item tab-title="我的" to="user" icon="my"></nut-tabbar-item>
    </nut-tabbar>
  </div>
</template>

<script>
export default {
  components: {},
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

</style>