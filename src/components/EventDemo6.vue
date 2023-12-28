<template>
    <h3>EVENT6</h3>

    <a @click.prevent="clickHandler" href="http://baidu.com">baidu</a>

    <div @click="clickDiv">
        <p @click.stop="clickP">test maopao</p>
    </div>
</template>


<script>
export default{
    data(){
        return{

        }
    },
    methods:{
        clickHandler(e){
            // e.preventDefault();
            console.log("asd");
        },
        clickDiv(){
            console.log("div");
        },
        clickP(e){
            console.log("p");
        }
    }
}

</script>