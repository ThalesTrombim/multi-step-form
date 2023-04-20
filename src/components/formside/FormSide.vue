<script lang="ts" setup>
import StepsIndicator from './components/StepsIndicator.vue';

interface StepsTypes {
  label: string,
  isActive: boolean
}

// PASSAR ISSO PARA UM STATE (PINIA) DEPOIS.
const steps: Array<StepsTypes> = [
  {
    label: 'your info',
    isActive: true
  },
  {
    label: 'select plan',
    isActive: true
  },
  {
    label: 'add-ons',
    isActive: true
  },
  {
    label: 'summary',
    isActive: true
  }
]

</script>

<template>
  <div class="form-side--container">
    <steps-indicator 
      v-for="(step, index) in steps"
      :key="index"
      :step="index+1"
      :label="step.label"
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