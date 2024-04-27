<script setup></script>

<template>
  <section id="hero-bg">
    <div class="ms-5 d-none d-sm-none d-md-none d-lg-none d-xl-none d-xxl-block">
      <slot name="bg-xxl"></slot>
    </div>
    <div class="d-none d-sm-none d-md-none d-lg-none d-xl-block d-xxl-none">
      <slot name="bg-xl"></slot>
    </div>
    <div class="d-none d-sm-none d-md-none d-lg-block d-xl-none d-xxl-none">
      <slot name="bg-lg"></slot>
    </div>
    <div class="d-none d-sm-none d-md-block d-lg-none d-xl-none d-xxl-none">
      <slot name="bg-md"></slot>
    </div>
    <div class="d-none d-sm-block d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="bg-sm"></slot>
    </div>
    <div class="d-block d-sm-none d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="bg-block"></slot>
    </div>
  </section>

  <section id="hero-images">
    <div class="text-center d-none d-sm-none d-md-none d-lg-none d-xl-none d-xxl-block">
      <slot name="image-xxl"></slot>
    </div>
    <div class="text-center d-none d-sm-none d-md-none d-lg-none d-xl-block d-xxl-none">
      <slot name="image-xl"></slot>
    </div>
    <div class="text-center d-none d-sm-none d-md-none d-lg-block d-xl-none d-xl-none d-xxl-none">
      <slot name="image-lg"></slot>
    </div>
    <div class="text-center d-none d-sm-none d-md-block d-lg-none d-xl-none d-xxl-none">
      <slot name="image-md"></slot>
    </div>
    <div class="text-center d-none d-sm-block d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="image-sm"></slot>
    </div>
    <div class="text-center d-block d-sm-none d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="image-block"></slot>
    </div>
  </section>

  <section id="hero-card">
    <div class="d-none d-sm-none d-md-none d-lg-none d-xl-none d-xxl-block">
      <slot name="card-xxl"></slot>
    </div>
    <div class="d-none d-sm-none d-md-none d-lg-none d-xl-block d-xxl-none">
      <slot name="card-xl"></slot>
    </div>
    <div class="d-none d-sm-none d-md-none d-lg-block d-xl-none d-xl-none d-xxl-none">
      <slot name="card-lg"></slot>
    </div>
    <div class="d-none d-sm-none d-md-block d-lg-none d-xl-none d-xxl-none">
      <slot name="card-md"></slot>
    </div>
    <div class="d-none d-sm-block d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="card-sm"></slot>
    </div>
    <div class="d-block d-sm-none d-md-none d-lg-none d-xl-none d-xxl-none">
      <slot name="card-block"></slot>
    </div>
  </section>
</template>
