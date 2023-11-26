<script setup>
useHead({
  htmlAttrs: "en",
  title: "Buildmania",
  meta: [{ name: "description", content: "My amazing site." }],
});
</script>

<template>
  <div>
    <TheHeader />
    <NuxtPage />
    <TheFooter />
  </div>
</template>
