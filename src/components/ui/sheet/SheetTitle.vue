<script setup lang="ts">
import { cn } from '@/lib/utils'

const props = defineProps<{
  class?: string
}>()
</script>

<template>
  <h3 :class="cn('text-lg font-semibold text-foreground', props.class)">
    <slot />
  </h3>
</template>
