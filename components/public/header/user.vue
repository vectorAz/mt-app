<template>
  <div class="m-user">
    <template v-if="islogin">
      欢迎您 <span class="user">{{ user }}</span>
        [<nuxt-link to="/exit">退出</nuxt-link>]
    </template>
    <template v-else> 
        <nuxt-link to="/login" class="login">立即登录</nuxt-link>
        <nuxt-link to="/register" class="register">注册</nuxt-link>
    </template>
  </div>
</template>
<script>
export default {
  data() {
    return {
      islogin: false,
      user: "Sora"
    };
  }
};
</script>
<style scoped></style>
