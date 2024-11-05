<template>
  <div>
    <Header />
    <main class="main">
      <NuxtPage />
    </main>
    <Footer />
  </div>
</template>

<script setup></script>

<style lang="scss">
body {
  margin: 0;
  display: flex;
  flex-direction: column;
  height: 100vh;
}

.main {
  overflow-y: auto;
  flex: 1;
}
</style>
