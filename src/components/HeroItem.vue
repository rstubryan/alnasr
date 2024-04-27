<script setup>
import MainLayout from '@/components/MainLayout.vue'
import BaseButtonLarge from '@/components/BaseButtonLarge.vue'
import ContainerComponent from '@/components/ContainerComponent.vue'
import ImageBreakpoint from '@/components/ImageBreakpoint.vue'
import HeroBackground from '@/components/icons/HeroBackground.vue'
import ReviewCard from '@/components/ReviewCard.vue'
</script>

<template>
  <ContainerComponent>
    <MainLayout>
      <template #hero-left>
        <div class="mb-5">
          <div class="mb-3">
            <span class="badge text-primary fw-semibold py-2 px-4 rounded-5 bg-secondary fs-6">
              <slot name="left-subheading-hero"></slot>
            </span>
          </div>
          <div class="mb-3">
            <h1 class="text-dark display-4 fw-bold">
              <slot name="left-heading-hero"></slot>
            </h1>
          </div>
          <div class="mb-4">
            <p class="lh-lg fs-5 fw-light"><slot name="left-desc-hero"></slot></p>
          </div>
          <BaseButtonLarge> <template #btn-text>Contact Us</template> </BaseButtonLarge>
        </div>
      </template>

      <template #hero-right>
        <ImageBreakpoint>
          <template #bg-xxl> <HeroBackground style="margin-top: 6rem"></HeroBackground></template>
          <template #bg-xl> <HeroBackground style="margin-top: 9rem"></HeroBackground></template>
          <template #bg-lg> </template>
          <template #bg-md> </template>
          <template #bg-sm> </template>
          <template #bg-block></template>
        </ImageBreakpoint>
        <div>
          <ImageBreakpoint>
            <template #card-xxl>
              <ReviewCard style="margin-left: 24rem; margin-top: 1rem"></ReviewCard>
              <ReviewCard style="margin-top: 18rem"></ReviewCard>
            </template>
            <template #card-xl>
              <ReviewCard style="margin-left: 19.7rem; margin-top: 1rem"> </ReviewCard>
              <ReviewCard style="margin-top: 25rem"></ReviewCard>
            </template>
            <template #card-lg>
              <ReviewCard style="margin-left: 14rem; margin-top: 1rem"> </ReviewCard>
              <ReviewCard style="margin-top: 20rem"></ReviewCard>
            </template>
            <template #card-md>
              <ReviewCard style="margin-left: 6.5rem; margin-top: 1rem"> </ReviewCard>
              <ReviewCard style="margin-top: 19rem"></ReviewCard>
            </template>
            <template #card-sm>
              <ReviewCard style="margin-left: 17rem; margin-top: 1rem"> </ReviewCard>
              <ReviewCard style="margin-top: 23rem"></ReviewCard>
            </template>
            <template #card-block>
              <ReviewCard style="margin-left: 6rem; margin-top: 1rem"> </ReviewCard>
              <ReviewCard style="margin-left: 0.5rem; margin-top: 20rem"></ReviewCard>
            </template>
          </ImageBreakpoint>
        </div>
        <ImageBreakpoint>
          <template #image-xxl>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-50" />
          </template>
          <template #image-xl>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-75" />
          </template>
          <template #image-lg>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-75" />
          </template>
          <template #image-md>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-100" />
          </template>
          <template #image-sm>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-75" />
          </template>
          <template #image-block>
            <img src="./images/HeroImages.jpg" alt="images-hero" class="rounded-4 w-100" />
          </template>
        </ImageBreakpoint>
      </template>
    </MainLayout>
  </ContainerComponent>
</template>
