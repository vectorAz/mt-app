<template>
    <div class="m-header">
        <el-row>
            <el-col>
                <topBar></topBar>
            </el-col>
        </el-row>
        <el-row>
            <el-col>
                <searchBar></searchBar>
            </el-col>
        </el-row>
    </div>
</template>
<script>
import topBar from './topbar';
import searchBar from './searchbar';
export default {
    components: {
        topBar,
        searchBar
    },
}
</script>
<style lang="scss">
@import "../../../assets/css/public/layout.scss";
@import "../../../assets/css/public/header.scss";
</style>