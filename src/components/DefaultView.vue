<script lang="ts" setup>
import FormWrapper from './FormWrapper.vue';
</script>

<template>
  <div class="default-view--container">
    <form-wrapper />
  </div>
</template>

<style lang="scss" scoped>
.default-view {
  &--container {
    background-color: #eff5ff;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 100%;
  }
}
</style>