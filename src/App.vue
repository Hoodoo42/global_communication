<template>
  <div id="app">
  <toast-notification></toast-notification>
  <delete-button></delete-button>
  <post-button></post-button>
  </div>
</template>

<script>
import ToastNotification from '@/components/ToastNotification.vue'
import DeleteButton from '@/components/DeleteButton.vue'
import PostButton from '@/components/PostButton.vue'

export default {
  name: 'App',
  components: {
 ToastNotification,
 DeleteButton,
 PostButton
  }
}
</script>

<style>

</style>
