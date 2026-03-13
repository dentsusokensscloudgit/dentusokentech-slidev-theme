<template>
  <div class="slidev-layout blank-layout">
    <slot />
  </div>
</template>

<style scoped>
.blank-layout {
  background-image: none !important;
  padding: 0;
}

.blank-layout::before,
.blank-layout::after {
  display: none !important;
}
</style>
