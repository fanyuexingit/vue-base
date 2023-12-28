<template>
    <h3>list</h3>

    <button @click="addHandle">add item</button>
    <ul>
        <li v-for="(item, index) in names" :key="index">{{ item }}</li>
    </ul>
</template>


<script>
export default {
    data() {
        return {
            names:["asd","qwe","zxc"]
        }
    },
    methods: {
        addHandle(){
            // this.names.push("sdafdfd");

            this.names = this.names.concat("sakura");
        }
    }
}

</script>