<template>
  <header class="header">
    <div class="centered _spaceBetween">
      <NuxtLink to="/">
        <h2 class="title">ШАПКА</h2>
      </NuxtLink>
      <select class="toggleTheme" v-model="$colorMode.preference">
        <option value="system">System</option>
        <option value="light">Light</option>
        <option value="dark">Dark</option>
        <option value="sepia">Sepia</option>
      </select>
    </div>
  </header>
</template>

<script setup></script>

<style lang="scss">
body {
  background-color: #fff;
  color: rgba(0, 0, 0, 0.8);
}

.main {
  padding: 1em;
  overflow-y: hidden;
}
.dark-mode body {
  background-color: #202020;
  color: #ebf4f1;
}
.sepia-mode body {
  background-color: #f1e7d0;
  color: #433422;
}
.header {
  display: flex;
  justify-content: space-between;
  background-color: aliceblue;
  color: #000000;
  padding: 15px 10px;
  position: fixed;
  left: 0;
  right: 0;
  z-index: 1000;
  top: 0;
  box-shadow: 5px 10px 10px -5px black;
}

.title {
  margin: 0;
}
</style>
