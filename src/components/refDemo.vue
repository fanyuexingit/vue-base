<template>
    <h3>ref</h3>

    <div ref="hhh">{{ content }}</div>

    <input type="text" ref="username">
    <button @click="getElementHandle">get it</button>

</template>

<script>
export default{
    data() {
        return {
            content: "xxx"
        }
    },
    methods:{
        getElementHandle() {
            this.$refs.hhh.innerHTML = "ooo"
            console.log(this.$refs.username.value)
        }
    }
}

</script>