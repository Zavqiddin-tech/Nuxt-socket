<script setup lang="ts">
const token = useCookie('testToken')

useHead({
  title: "dashboard",
});
definePageMeta({
  middleware: [
    function (to, from) {
      // Custom inline middleware
    },
    'admin',
  ],
});
</script>

<template>
  dashboard
  <UButton>Click</UButton>
  {{ token }}
</template>

<style lang="scss"></style>