<template>
    <div>
<button @click="delete_click" >Delete</button>
    </div>
</template>

<script>
    export default {
data() {
    return {
        message: `successfully deleted`
    }
},

        methods: {
            delete_click() {
                this.$root.$emit(`toast_notify`, this.message )
            }
        },
    }
</script>

<style scoped>

</style>