<script setup>
import Account from "./components/Account.vue";
import Auth from "./components/Auth.vue";

const user = useSupabaseUser();
</script>

<template>
  <div class="container" style="padding: 50px 0 100px 0">
    <Account v-if="user" />
    <Auth v-else />
  </div>
</template>
