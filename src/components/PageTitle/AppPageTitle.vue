<script setup>
import AppButton from '../Button/AppButton.vue'
import AppInput from '../Input/AppInput.vue'
import SearchIcon from '../icons/SearchIcon.vue'
</script>

<template>
  <section class="layout-spacing">
    <div>
      <h1>Seus favorecidos</h1>
      <AppButton class="page-title__button" />
    </div>
    <AppInput class="page-title__input">
      <template #suffix>
        <SearchIcon class="suffix" />
      </template>
    </AppInput>
  </section>
</template>

<style scoped>
section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: var(--gray-500);
  height: 122px;
  background-color: var(--gray-600);
}

section div {
  display: flex;
}

h1 {
  font-weight: 300;
}

.page-title__button {
  margin-left: 14px;
  cursor: pointer;
}

.page-title__input {
  height: 31px;
  width: 254px;
}
</style>
