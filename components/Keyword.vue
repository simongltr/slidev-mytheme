<script setup lang="ts">
defineProps<{
  color?: 'red' | 'orange' | 'amber' | 'yellow' | 'lime' | 'green' | 'emerald' | 'teal' | 'cyan' | 'sky' | 'blue' | 'indigo' | 'violet' | 'purple' | 'fuchsia' | 'pink' | 'rose'
}>()
</script>

<template>
  <span class="keyword" :class="color ?? 'blue'"><slot /></span>
</template>

<style scoped>
.keyword {
  @apply px-1.5 py-0.5 rounded font-medium;
}
.red { @apply bg-red-500/12 text-red-600; }
.orange { @apply bg-orange-500/12 text-orange-600; }
.amber { @apply bg-amber-500/12 text-amber-600; }
.yellow { @apply bg-yellow-500/12 text-yellow-600; }
.lime { @apply bg-lime-500/12 text-lime-600; }
.green { @apply bg-green-500/12 text-green-600; }
.emerald { @apply bg-emerald-500/12 text-emerald-600; }
.teal { @apply bg-teal-500/12 text-teal-600; }
.cyan { @apply bg-cyan-500/12 text-cyan-600; }
.sky { @apply bg-sky-500/12 text-sky-600; }
.blue { @apply bg-blue-500/12 text-blue-600; }
.indigo { @apply bg-indigo-500/12 text-indigo-600; }
.violet { @apply bg-violet-500/12 text-violet-600; }
.purple { @apply bg-purple-500/12 text-purple-600; }
.fuchsia { @apply bg-fuchsia-500/12 text-fuchsia-600; }
.pink { @apply bg-pink-500/12 text-pink-600; }
.rose { @apply bg-rose-500/12 text-rose-600; }
</style>
