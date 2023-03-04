<script lang="ts" setup>
interface PropsTypes {
  step: number
  label: string,
  isActive: boolean
}

withDefaults(defineProps<PropsTypes>(), {
  isActive: false
});
</script>

<template>
  <div class="steps-indicator--container">
    <div class="steps-indicator--counter" :class="{ 'is-active' : isActive }">1</div>
    <div>
      <span>Step {{ step }}</span>
      <p>{{ label }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.is-active {
  background-color: #bee1ff;
  color: #000;
}
.steps-indicator {
  &--container {
    display: flex;
    align-items: center;
    gap: 16px;
    text-transform: uppercase;
    color: #bee1ff;

    span {
      font-size: 12px;
      font-weight: 300;
    }
    p {
      margin-top: 4px;
      font-weight: 500;
    }
  }
  &--counter {
    padding: 10px 15px;
    border: 1px solid #bee1ff;
    border-radius: 100%;
  }
}
</style>