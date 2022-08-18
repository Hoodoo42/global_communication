<template>
    <div>
<button @click="post_message">POST</button>
    </div>
</template>

<script>
    export default {
        methods: {
           post_post () {
                    this.$root.$emit(`toast_notify`, this.post_post)
            }
        },
    
    }
</script>

<style scoped>

</style>