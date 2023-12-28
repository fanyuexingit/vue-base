<template>
    <h3>EVENT3</h3>

    <button @click="addCount">add</button>
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
        addCount(e){
            e.target.innerHTML = "add" + this.count;
            this.count++;
        }
    }
}
</script>