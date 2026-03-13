<template>
  <div class="slidev-layout cover">
    <slot />
    <img src="/logo.png" class="cover-logo" />
  </div>
</template>

<style scoped>
.cover {
  background-image: none !important;
  padding: 80px 40px 200px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  overflow: visible !important;
}

.cover::before,
.cover::after {
  display: none !important;
}

.cover :deep(h1) {
  font-size: 42px !important;
  margin-top: 0;
}

.cover :deep(h1)::before {
  content: "";
  display: block;
  width: 150px;
  height: 10px;
  margin-bottom: 8px;
  background: var(--color-accent1);
}

.cover :deep(p) {
  font-size: 18px;
  color: var(--color-dk2);
}

.cover-logo {
  position: absolute;
  bottom: 5px;
  left: 30px;
  width: 140px;
  height: auto;
  z-index: 10;
}
</style>
