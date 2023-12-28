<template>
    <h3>EVENT2</h3>

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
        addCount(){
            this.count++;
        }
    }
}
</script>