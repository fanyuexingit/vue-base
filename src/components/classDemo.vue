<template>

<h3>class</h3>
<p :class="{ 'active': isActive, 'text-danger': hasError }">class1</p>
<p :class="classObject">class2</p>
<p :class="[arrActive, arrHasError]">class3</p>

</template>


<script>
export default {
    data() {
        return {
            isActive: true,
            hasError: true,

            classObject:{
                'active': true,
                'text-danger': true
            },
            
            arrActive: "active",
            arrHasError: "text-danger"
        }
    }
}

</script>

<style>

.active{
    color:red;
    font-size: 30px;
}

.text-danger{
    color: #000;
}
</style>