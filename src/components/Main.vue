<template>
    <div class="view-container">
        <div class="app-contain">
            <div class="form-container">
                <div class="filter-view">
                    <el-input v-model="filterText" placeholder="请输入搜索内容" class="filter-input">
                        <template #prepend>
                            <el-icon ><Search /></el-icon>
                        </template>
                    </el-input>
                    <el-button type="primary" @click="handleCreate">创建问卷</el-button>

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

<script>

import {Search} from "@element-plus/icons-vue";
import {ElButton, ElInput} from "element-plus";
import {defineComponent, reactive} from "vue";

export default defineComponent({
    components: {
        ElInput,
        ElButton
    },
    setup() {
        const filterText = reactive({
            filterText: ""
        })

        const handleCreate = () => {
            console.log("创建问卷")
        }

        return {
            filterText,
            handleCreate
        }
    }
})




</script>

<style>

.filter-view {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;

}

.filter-input {
    width: 100px;
}

.card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
}



</style>