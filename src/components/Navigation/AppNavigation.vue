<template>
  <nav class="layout-spacing">
    <ul>
      <li>Seus favorecidos</li>
    </ul>
  </nav>
</template>

<style scoped>
nav {
  height: 50px;
  background-color: var(--green-300);
  color: var(--white);
  display: flex;
}

ul {
  list-style-type: none;
  height: 100%;
}

li {
  position: relative;
  height: 100%;
  display: flex;
  align-items: center;
  cursor: pointer;
}

li::after {
  content: '';
  display: block;
  position: absolute;
  bottom: 0;
  width: 110%;
  border-bottom: 3px solid var(--white);
}
</style>
