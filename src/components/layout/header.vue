<template>
  <div class="headers">
    <div class="logo">
      <img src="@/assets/logo/comesit_logo.png" />
    </div>
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#FFF0B0"
      text-color="#D29375"
      active-text-color="#93B9D5"
    >
      <el-menu-item index="1">首頁</el-menu-item>
      <el-submenu index="2">
        <template slot="title">我的工作台</template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
        <el-submenu index="2-4">
          <template slot="title">选项4</template>
          <el-menu-item index="2-4-1">选项1</el-menu-item>
          <el-menu-item index="2-4-2">选项2</el-menu-item>
          <el-menu-item index="2-4-3">选项3</el-menu-item>
        </el-submenu>
      </el-submenu>
      <el-menu-item index="3">登入</el-menu-item>
      <el-menu-item index="4">
        <a href="https://www.ele.me" target="_blank">購物車</a>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: "headers",
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.logo {
  height: 190px;
  width: 200px;
  margin: auto;
  img {
    width: 100%;
    height: 100%;
  }
}
</style>
