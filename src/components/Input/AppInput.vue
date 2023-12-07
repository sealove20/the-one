<template>
  <div>
    <input v-bind="$attrs" placeholder="Nome, CPF, agência ou conta" />
    <slot name="suffix"></slot>
  </div>
</template>

<style scoped>
div {
  position: relative;
}

input {
  font-size: var(--14px);
  font-weight: 300;
  color: var(--gray-500);
  outline: none;
  border: none;
  border-radius: 3px;
  padding-left: 5px;
  width: 100%;
}

input::placeholder {
  font-size: var(--14px);
  font-weight: 300;
}

:slotted(.suffix) {
  position: absolute;
  top: 8px;
  right: 10px;
}
</style>
