<template>
<h3>watch</h3>
<p>{{ message }}</p>
<button @click="updateHandle">update message</button>


</template>


<script>
export default {
    data() {
        return{
            message: "hello"
        }
    },
    methods: {
        updateHandle(){
            this.message = "world"
        }
    },
    watch: {
        message(newValue, oldValue){
            console.log(newValue, oldValue)
        }
    }
}

</script>