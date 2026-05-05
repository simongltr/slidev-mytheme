<script setup lang="ts">
defineProps<{
  color?: 'red' | 'orange' | 'amber' | 'yellow' | 'lime' | 'green' | 'emerald' | 'teal' | 'cyan' | 'sky' | 'blue' | 'indigo' | 'violet' | 'purple' | 'fuchsia' | 'pink' | 'rose'
}>()
</script>

<template>
  <div class="callout" :class="color ?? 'blue'">
    <slot />
  </div>
</template>

<style scoped>
.callout {
  @apply border-l-3 pl-4 py-2 my-4 rounded-r-md;
}
.red { @apply border-red-500 bg-red-500/7; }
.orange { @apply border-orange-500 bg-orange-500/7; }
.amber { @apply border-amber-500 bg-amber-500/7; }
.yellow { @apply border-yellow-500 bg-yellow-500/7; }
.lime { @apply border-lime-500 bg-lime-500/7; }
.green { @apply border-green-500 bg-green-500/7; }
.emerald { @apply border-emerald-500 bg-emerald-500/7; }
.teal { @apply border-teal-500 bg-teal-500/7; }
.cyan { @apply border-cyan-500 bg-cyan-500/7; }
.sky { @apply border-sky-500 bg-sky-500/7; }
.blue { @apply border-blue-500 bg-blue-500/7; }
.indigo { @apply border-indigo-500 bg-indigo-500/7; }
.violet { @apply border-violet-500 bg-violet-500/7; }
.purple { @apply border-purple-500 bg-purple-500/7; }
.fuchsia { @apply border-fuchsia-500 bg-fuchsia-500/7; }
.pink { @apply border-pink-500 bg-pink-500/7; }
.rose { @apply border-rose-500 bg-rose-500/7; }
</style>
