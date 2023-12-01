<script setup>
import Auth from '~/components/Auth.vue'
import Account from '~/components/Account.vue'
const user = useSupabaseUser();
</script>

<template>
    <div class="container" style="padding: 50px 0 100px 0">
        <Home v-if="user" />
        <Auth v-else />
    </div>
</template>