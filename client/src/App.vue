<template>
  <el-container>
    <el-header class="flex text-black bg-blue-500 font-bold justify-center items-center mb-4">标题栏</el-header>
    <el-container class="h-screen">
        <el-aside class="w-48">
          <el-menu
            class="el-menu-vertical-demo w-48"
            default-active="1">
            <el-submenu index="1"> 
              <template #title>
                <span>资产总览</span>
              </template>
              <el-menu-item-group >
                <el-menu-item index="1-1" >政法委arm</el-menu-item>
                <el-menu-item index="1-2" >政法委非arm</el-menu-item>
                <el-menu-item index="1-3" >辅助办案</el-menu-item>
                <el-menu-item index="1-4" >涉案财物</el-menu-item>
              </el-menu-item-group>
            </el-submenu>
            <el-menu-item index="2">
              <template #title>资产查询</template>
            </el-menu-item>
            <el-menu-item index="3">
              <template #title>资产编辑</template>
            </el-menu-item>
          </el-menu>
        </el-aside>
        <el-main class="bg-purple-400 text-black">正文部分</el-main>
    </el-container>
  </el-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'App',
  components: {
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #409EFF;
  margin-top: 60px;
}

.el-menu-vertical-demo {
  width: 30%;
}
</style>
