<script setup lang="ts">
import { RouterView } from 'vue-router'
import Header from './components/HeaderDefault.vue'
import Footer from './components/FooterDefault.vue'
</script>

<template>
  <Header class="header-main" />
  <RouterView class="main-view" />
  <Footer class="footer-main" />
</template>

<style lang="scss" scoped>
.header-main {
  position: fixed;
}
.main-view {
  height: 100vh;
  padding: 0;
}

.footer-main {
  margin-top: 20px;
}
</style>
