<template>
    <h3>EVENT5</h3>

    <p @click="getNameHandler(item, $event)" v-for="(item, index) of names">{{ item }}</p>
</template>


<script>
export default{
    data(){
        return{
            names: ["qwe","asd","zcx"]
        }
    },
    methods:{
        getNameHandler(item, e){
            console.log(item + e.target.innerHTML);
        }
        
    }
}
</script>