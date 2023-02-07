<script lang="ts" setup>
import FormSide from './formside/FormSide.vue';
</script>

<template>
  <div class="form-wrapper--container">
    <form-side />
  </div>
</template>

<style lang="scss" scoped>
.form-wrapper {
  &--container {
    background-color: #FFF;
    padding: 10px;
    border-radius: 10px;
    display: flex;
  }
}
</style>