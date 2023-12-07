<template>
    <div class="header">
        <div class="header-wrapper">
        <div class="header-left" width="200px">
            <router-link to="/home">
            <img src="../assets/logo.svg" alt="logo" />
            </router-link>
        </div>
        <div class="header-right">
            <div class="header-right-item">
                
            </div>
        </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="less" scoped>
.header-left img {
  width: 180px; /* 调整图片的宽度 */
  height: 60px; /* 调整图片的高度 */
  background-size: cover; /* 或者使用 background-size: contain; */
  margin: auto;
}

</style>

