<template>
  <div class="home">
    <header class="header auto-width">
      <div class="search"></div>
    </header>
    <section class="container item-one auto-container"></section>
    <section class="container item-one auto-container"></section>
    <section class="container item-one auto-container"></section>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({
  components: {}
})
export default class Home extends Vue {}
</script>

<style lang="scss" scoped>
.home {
  display: flex;
  align-items: center;
  flex-direction: column;
  background-color: #f3f3f3;
}
.header {
  max-width: 960px;
  width: 90%;
  background-color: #fff;
  box-shadow: 0 0 15px rgba(100, 100, 100, 0.1);
  overflow: hidden;
  border-radius: 10px;
}
.container {
  max-width: 960px;
  overflow: hidden;
  width: 90%;
  height: 200px;
  background-color: #fff;
}
.item-one {
  border-radius: 10px;
  box-shadow: 0 0 15px rgba(100, 100, 100, 0.1);
}
@media screen and (min-width: 992px) {
  .auto-width {
    height: 560px;
    margin-bottom: 15px;
  }
  .auto-container {
    margin: 15px 0;
  }
}
@media screen and (max-width: 992px) and (min-width: 768px) {
  .auto-width {
    height: 460px;
    margin-bottom: 10px;
  }
  .auto-container {
    margin: 10px 0;
  }
}

@media screen and (max-width: 768px) {
  .auto-width {
    height: 260px;
    margin-bottom: 5px;
  }
  .auto-container {
    margin: 5px 0;
  }
}
</style>