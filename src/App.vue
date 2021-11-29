<template>
  <div id="app">
    <amap :zoom="15" :center="position">
      <amap-marker
          :position="position"
          :label="{
          content: 'Hello, AMap-Vue!',
          direction: 'bottom',
        }"
          draggable
      />
    </amap>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      position: [116.473179, 39.993169]
    };
  }
};
</script>

<style>
html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>

<style lang="less" scoped>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  height: 100%;
}
</style>
