<template>
    <div class="view-container">
        <div class="app-contain">
            <div class="form-container">
                <div class="filter-view">
                    <!-- <el-input v-model="filterText" placeholder="请输入问卷名称" class="filter-input">
                        <template #prepend>
                            <el-icon ><Search /></el-icon>
                        </template>
                    </el-input> -->
                    <input v-model="form.filter" type="text" class="filter-input" placeholder="请输入问卷名称">
                    <el-button type="primary" :icon="Search" class="filter-button">搜索</el-button>
                    <el-button type="primary" :icon="Plus" @click="handleCreate">创建问卷</el-button>

                </div>
                <div class="project-container">
                    <div class="card-container">

                    </div>
                    <div class="page-contain">
                        <div class="page">

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import {Search, Plus} from "@element-plus/icons-vue";
import {ElButton, ElInput} from "element-plus";
import { reactive } from 'vue';

const form = reactive({
  filter: '',
});


</script>

<style>

.filter-view {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 20px;
}

.filter-input {
    width: 300px;
    height: 36px;
    border-radius: 5px;
    border: 1px solid #e3e3e3;
    padding: 10px;
    box-sizing: border-box;
    outline: none;
    transition: 0.3s;
    margin-left: 0;
    margin-right: 20px;
}

.filter-input:focus {
    border: 1px solid #806ac4;
}

.filter-button {
    margin-right: 100px; 
}

.card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}



</style>