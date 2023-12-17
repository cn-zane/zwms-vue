<template>
    <router-view/>
<!--    <el-button type="primary" @click="handleLogin">测试登录</el-button>-->
<!--    <el-button type="danger" @click="handleUserRequest">测试获取用户请求</el-button>-->
</template>

<script setup>
import requestUtil from '@/util/request'
import store from "@/store";

// const handleLogin = async ()=>{
//     requestUtil.get('test/login').then((resp)=>{
//         let data = resp.data;
//         if (data.code === 200) {
//             const token = data.token;
//             console.log("登录成功,token:", token);
//             store.commit('SET_TOKEN', token);
//         }else{
//             console.log("登录出错")
//         }
//     })
// }
// const handleUserRequest = async ()=>{
//     requestUtil.get('test/userList').then((resp)=>{
//         let data = resp.data;
//         if (data.code === 200) {
//             const userList = data.userList;
//             console.log("用户列表:", userList);
//         }
//     })
// }
</script>

<style>
html,body,#app{
    height: 100%;
}

.app-container{
    padding:20px
}
</style>
