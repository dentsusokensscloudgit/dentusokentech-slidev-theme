<template>
  <div class="slidev-layout dstech-section">
    <slot />
  </div>
</template>

<style scoped>
.dstech-section {
  background-color: var(--color-dk2) !important;
  background-image: none !important;
  color: var(--color-lt1);
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 80px;
}

.dstech-section::before,
.dstech-section::after {
  display: none !important;
}

.dstech-section :deep(h1) {
  color: var(--color-lt1);
  font-size: 40px !important;
}
</style>
