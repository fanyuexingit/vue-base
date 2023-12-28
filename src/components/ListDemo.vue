<template>
    <h3>List parse</h3>
    <P v-for="(item, index) in names">{{ item }} - {{ index }}</P>

    <div v-for="item in result" :key="item.id">
        <p>{{ item.id }}</p>
        <src :image="item.avator">{{ item.title }}</src>
    </div>

    <div>
        <p v-for="(item,key,index) of userInfo">
            {{ item }}--{{ key }}--{{ index }}</p>
    </div>
</template>

<script>
export default{
    data(){
        return{
            names:["sad","qwe","zxc"],
            result:[
                {
                    "id": 123,
                    title: "123123",
                    avator: "123123123"
                },
                {
                    "id": 456,
                    title: "456456",
                    avator: "456456456"
                },
                {
                    "id": 789,
                    title: "789789",
                    avator: "789789789"
                }
            ],
            userInfo:{
                name:"fan",
                sex: "male",
                age: "18"
            }
        }
    }
}

</script>