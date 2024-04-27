<script setup>
import { ref } from 'vue'
import BaseButtonLarge from '@/components/BaseButtonLarge.vue'
import AppLogo from '@/components/icons/AppLogo.vue'

const navLinks = ref([
  { text: 'Home', path: '/' },
  { text: 'About Us', path: '/about' },
  { text: 'Package', path: '/package' },
  { text: 'Facilities', path: '/facilities' },
  { text: 'Gallery', path: '/gallery' }
])
</script>
<template>
  <div class="container mt-5">
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">
          <AppLogo></AppLogo>
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mx-auto mb-2 mb-lg-0 gap-3">
            <li class="nav-item" v-for="item in navLinks" :key="item.text">
              <a class="nav-link" href="#">{{ item.text }}</a>
            </li>
          </ul>
          <BaseButtonLarge href="https://www.google.com" target="_blank">
            <template #btn-text>Contact Us</template>
          </BaseButtonLarge>
        </div>
      </div>
    </nav>
  </div>
</template>

<style scoped></style>
