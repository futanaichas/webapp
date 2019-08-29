<template>
  <div class="Index">
    <h1>这是奶茶大大的小论坛</h1>
    <header>
        <ul>
            <li>首页</li>
            <li>漫画</li>
            <li>里番</li>
            <li>3D</li>
            <li>GAL</li>
        </ul>
    </header>
    
  </div>
</template>

<script>
export default {
  name: 'Index',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul{
  display: flex;
  justify-content:space-around;
}
ul li{
    height: 40px;
  list-style: none;
    color:#Fff;
    background-color: black;
    flex-grow:1;
    line-height: 40px;
    align-items: center;
}
</style>
