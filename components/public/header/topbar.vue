<template>
    <el-row :gutter="0">
      <el-col :span="5"><Geo /> </el-col>
      <el-col :span="5" ><User /></el-col>
      <el-col :span="13"><Nav /></el-col>
    </el-row>
</template>
<script>
import Geo from "./geo";
import User from "./user";
import Nav from "./nav";
export default {
  components: {
    Geo,
    User,
    Nav
  }
};
</script>
<style >

</style>
