<script>
    export default{
        name :'LoOp',
        data(){
            return{
                i:0,
                containt:[
                    "buoun",
                    "kumar"
                ]
            }
        }


    }
</script>

<style>

</style>

<template>
    <h1>Loop</h1>
    <p v-for="(data,index) in containt" :key="index">{{ data }}</p>
</template>