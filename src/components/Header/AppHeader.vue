<script setup>
import TransfeeraIcon from '../icons/TransfeeraIcon.vue'
</script>

<template>
  <header class="layout-spacing">
    <i>
      <TransfeeraIcon />
    </i>
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  width: 100%;
  height: 2rem;
  margin-top: 10px;
}

i {
  display: flex;
  place-items: center;
  place-content: center;
  width: 128px;
  height: 25px;
}

@media (max-width: 640px) {
  header {
    justify-content: center;
  }
}
</style>
