<script setup lang="ts">
import { ref, defineProps } from 'vue'

const props = defineProps({
  value: {
    default: false,
  },
  true: {
    default: 'true',
  },
  false: {
    default: 'false',
  },
  trueClass: {
    default: 'text-$c-brand',
  },
  falseClass: {
    default: 'text-orange-400',
  },
})
</script>

<template>
  <span :class="props.value ? props.trueClass : props.falseClass">
    {{ props.value ? props.true : props.false }}
  </span>
</template>
