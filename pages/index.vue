<template>
  <VNavigationDrawer :model-value="true" location="right">
    Drawer 2
  </VNavigationDrawer>
</template>

<script setup lang="ts">
onServerPrefetch(async () => {
  // Removing this makes the hydration mismatch go away.
  await new Promise((resolve) => setTimeout(resolve, 500));

  // Use case:
  // await myTanStackQuery.suspense();
});
</script>
