<template>
    <el-button type="danger" @click="testHandler">测试接口</el-button>
    <el-button type="danger" @click="testLogoutHandler">登出接口</el-button>
</template>

<script setup>
import requestUtil from '@/util/request'


const testHandler=async ()=>{
    let result=await requestUtil.get("test/userList");
    console.log(result)

}
const testLogoutHandler=async ()=>{
    let result=await requestUtil.get("logout");
}
</script>

<style scoped>

</style>
