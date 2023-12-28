<template>
    <H3>IF parse</H3>

    <div v-if="flag">can you see me</div>
    <div v-else>see me</div>

    <div v-if="type === 'A'">A</div>
    <div v-else-if="type === 'B'">B</div>
    <div v-else-if="type === 'C'">C</div>
    <div v-else>not A B C</div>

    <div v-show="flag">can you see me</div>
</template>


<script>
export default{
    data(){
        return{
            flag:true,
            type:"B"
        }
    }
}

</script>