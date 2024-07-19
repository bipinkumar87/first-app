<template>
    <li class="text-danger"><a href="">q</a></li>
    <li><a href="">{{ fname }}</a></li>
    <li><a href="">{{ uId }}</a></li>
    <button class="btn btn-danger py-3 px-2 mx-3" @click="dangerMsg">click me</button>
    <button class="btn btn-primary py-3 px-4" @click="askMe">askme</button>
</template>
<script>
export default{
    name:'NevBar',
    methods:{
        askMe(){
            alert("askme naj");
        },
        dangerMsg(){
            alert("this is danger");
        }
    },
    data(){
        return{
            fname:"bipin",
            uId:123
        }
    }
}
</script>
<style>
    @import'~bootstrap/dist/css/bootstrap.css';
</style>