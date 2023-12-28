<template>
    <h3>EVENT1</h3>

    <button v-on:click="count++">add</button>
    <button @click="count++">add</button>
    <p>{{ count }}</p>
</template>


<script>
export default{
    data(){
        return{
            count:0
        }
    }
}
</script>