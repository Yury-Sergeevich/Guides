<template>
  <footer class="footer">
    <div class="centered _spaceBetween">
      <h2 class="title">ПОДВАЛ</h2>
      <NuxtLink to="/categories">перейти</NuxtLink>
    </div>
  </footer>
</template>

<script setup></script>

<style lang="scss">
.footer {
  background-color: aliceblue;
  padding: 15px 10px;
  color: #000000;
  position: fixed;
  left: 0;
  right: 0;
  z-index: 1000;
  bottom: 0;
}

.title {
  margin: 0;
}
</style>
