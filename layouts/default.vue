<template>
  <div class="layout">
    <!-- <AppHeader /> -->
    <div class="content"><slot /></div>
    <AppFooter />
  </div>
</template>

<style scoped>
.layout,
.content {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.layout {
  overflow-y: auto;
}

.content {
  /* margin-top: 64px; */
  overflow: hidden;
}
</style>

<style>
.page-enter-active,
.page-leave-active {
  transition: opacity 0.2s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
}
</style>
