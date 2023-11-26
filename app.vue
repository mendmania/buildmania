<script setup>
useHead({
  htmlAttrs: {
    lang: "en",
  },
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
