<template>
    <h3>EVENT4</h3>

    <button @click="addCount('hello')">add</button>
    <p>{{ count }}</p>
</template>


<script>
export default{
    data(){
        return{
            count:0
        }
    },
    methods:{
        addCount(msg){
            // e.target.innerHTML = "add" + this.count;
            console.log(msg);
            this.count++;
        }
    }
}
</script>