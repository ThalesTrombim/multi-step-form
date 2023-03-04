<script lang="ts" setup>
import StepsIndicator from './components/StepsIndicator.vue';
</script>

<template>
  <div class="form-side--container">
    <steps-indicator 
      :step="1"
      label="your info"
      :is-active="true"
    />
  </div>
</template>

<style lang="scss" scoped>
.form-side {
  &--container {
    background-image: url('../../assets/images/bg-sidebar-desktop.svg');
    padding: 25px;
    display: flex;
    height: 500px;
  }
}
</style>