<template>
    <h3>{{ person.name }}</h3>

    <p>{{ personContent }}</p>

    <p>{{ personContents() }}</p>
</template>

<script>
export default {
    data() {
        return{
            person: {
                name: "fyx",
                content: ['java', 'python', 'html']
            }
        }
    },
    computed: {
        personContent() {
            return this.person.content.length > 0 ? 'yes' : 'no'
        }
    },
    methods: {
        personContents() {
            return this.person.content.length > 0 ? 'yes' : 'no'
        }
    }
}
</script>