<script setup>
import MainLayout from '@/components/MainLayout.vue'
import BaseButtonLarge from '@/components/BaseButtonLarge.vue'
import ContainerComponent from '@/components/ContainerComponent.vue'
</script>

<template>
  <ContainerComponent>
    <MainLayout>
      <template #hero-left>
        <div class="mb-3">
          <span class="badge text-primary fw-semibold py-2 px-4 rounded-5 bg-secondary fs-6">
            <slot name="left-subheading-hero"></slot>
          </span>
        </div>
        <div class="mb-3">
          <h1 class="text-dark display-5 fw-bold">
            <slot name="left-heading-hero"></slot>
          </h1>
        </div>
        <div class="mb-3">
          <p class="lh-base"><slot name="left-desc-hero"></slot></p>
        </div>
        <BaseButtonLarge> <template #btn-text>Contact Us</template> </BaseButtonLarge>
      </template>
      <template #hero-right>
        <div></div>
      </template>
    </MainLayout>
  </ContainerComponent>
</template>
