<script setup>
const user = useSupabaseUser()
</script>

<template>
  <div>
    <Account v-if="user" />
    <Auth v-else />
  </div>
</template>
