<template>
  <div class="search-panel">
    <el-row class="m-header-searchbar">
      <el-col class="left" :span="4">
        <img
          src="//s0.meituan.net/bs/fe-web-meituan/fa5f0f0/img/logo.png"
          alt="美团"
        />
      </el-col>
      <el-col class="center" :span="14">
        <div class="wrapper">
          <el-input
            placeholder="搜索商家或地点"
            @focus='ishotPlace=true'
            @blur="ishotPlace=false"
          ></el-input>
          <button class="el-button el-button-primary">
            <i class="el-icon-search"></i>
          </button>
          <dl class="hotPlace" v-show="ishotPlace">
            <dt>热门搜索</dt>
            <dd>海底捞</dd>
            <dd>海底捞</dd>
            <dd>海底捞</dd>
            <dd>海底捞</dd>
          </dl>
          <!-- <dl class="searchList" v-show="issearchList">
            <dt>相关推荐</dt>
            <dd>火锅</dd>
            <dd>火锅</dd>
            <dd>火锅</dd>
            <dd>火锅</dd>
          </dl> -->
        </div>
        <p class="suggest">
          <a href="/">巴厘岛</a>
          <a href="/">巴厘岛</a>
          <a href="/">巴厘岛</a>
          <a href="/">巴厘岛</a>
        </p>
      </el-col>
      <el-col class="right" :span="6">
        <ul class="security">
          <li><i class="refund"></i></li>
          <li><i class="single"></i></li>
          <li><i class="overdue"></i></li>
        </ul>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data() {
    return {
      ishotPlace: false,
     issearchList:false
    };
  }
};
</script>
<style lang="scss">
@import "../../../assets/css/public/header/search.scss";
</style>
