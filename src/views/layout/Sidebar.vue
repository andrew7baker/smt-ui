<template>
    <el-menu mode="vertical"  unique-opened theme="dark" :default-active="$route.path" :collapse="true" background-color="#304156" text-color="#bfcbd9" active-text-color="#FFFFFF">
      <sidebar-item :routes='routes'></sidebar-item>
    </el-menu>
</template>

<style scoped>
  .el-submenu__title:hover {
    background-color: rgb(67, 74, 80);
  }
</style>

<script>
  import SidebarItem from './SidebarItem';
  export default {
    components: { SidebarItem },
    data() {
      return {
        routes: [{
          title: '例子',
          icon: 'setting'
        }]
      }
    }
  }
</script>
