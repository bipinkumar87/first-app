<script>
export default{
    name : 'DireCtive',
    data(){
        return{
            //  x:1,
            //  y:2,
            //  result:0
            show:false,
            keyword: ""
        }
    },
     methods : {
        toggle(){
            this.show=!this.show
        }
    //     add(){
    //         let x=this.x;
    //         let y=this.y;
    //         //this.result=x+y;
    //         //let results=x+y;
    //         let results=x+y;
    //         this.result=results;
    //         //alert(x+y)

    //     }
     }
}
</script>

<style>
@import "~bootstrap/dist/css/bootstrap.min.css";
</style>

<template>
    <!-- <p>{{ result }}</p>
    <button @click="add">add</button>
     //DireCtive 
    <h1 v-if="4===5">4 == 5</h1>
    <h1 v-else>4!=5</h1> -->
    <h1>gm</h1>
    <button class="btn btn-primary" @click="toggle()" >toggle</button>
     <img src="../assets/logo.png" alt="" v-if="show">
    <input type="text" v-model="keyword">
    <h1>{{ keyword }}</h1>
</template>