<script setup>
const user = useSupabaseUser()
import Auth from '~/components/Auth.vue'
import Home from '~/views/Home.vue'

</script>

<template>
  <div class="container" style="padding: 50px 0 100px 0">
    <Home v-if="user" />
    <Auth v-else />
  </div>
</template>