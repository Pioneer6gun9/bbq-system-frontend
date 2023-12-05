<template>
    <div class="header">
        <div class="header-wrapper">
        <div class="header-left">
            <router-link to="/home">
            <img src="../assets/logo.png" alt="logo" />
            </router-link>
        </div>
        </div>
    </div>
</template>


<script setup>
import { defineProps } from 'vue'
import { User } from '@element-plus/icons-vue'
import { ElMessage } from 'element-plus'
import { post } from '@/net'
import { reactive } from 'vue'
import router from '@/router'
</script>

<style scoped>
.header {
    width: 100%;
    height: 60px;
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    position: fixed;
    top: 0;
    left: 0;
    z-index: 999;
}

.header-wrapper {
    width: 70vw;
    height: 100%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>