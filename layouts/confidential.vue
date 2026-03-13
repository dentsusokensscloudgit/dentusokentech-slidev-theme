<template>
  <div class="slidev-layout default confidential">
    <div class="confidential-mark">CONFIDENTIAL</div>
    <slot />
  </div>
</template>

<style scoped>
.confidential-mark {
  font-size: 14px;
  font-weight: bold;
  color: var(--color-accent2);
  position: absolute;
  top: 12px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 10;
}
</style>
