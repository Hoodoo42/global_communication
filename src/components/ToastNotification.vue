<template>
    <div>
<h4 ref="message_display"></h4>
    </div>
</template>

<script>
    export default {
        methods: {
            display_message(message) {
                this.$refs[`message_display`][`innerHTML`] = message + `<button class="clear" @click="clear_message">dismiss</button>`;

            },
               clear_message() {
                this.$refs[`message_display`][`innerText`] = ``;
            }
        },
     
         
        

        mounted () {
            this.$root.$on(`toast_notify`, this.display_message);
        },
    }
</script>

<style scoped>

</style>