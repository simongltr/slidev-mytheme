<script setup lang="ts">
defineProps<{
  color?: 'red' | 'orange' | 'amber' | 'yellow' | 'lime' | 'green' | 'emerald' | 'teal' | 'cyan' | 'sky' | 'blue' | 'indigo' | 'violet' | 'purple' | 'fuchsia' | 'pink' | 'rose'
}>()
</script>

<template>
  <div class="box" :class="color ?? 'blue'">
    <slot />
  </div>
</template>

<style scoped>
.box {
  @apply border rounded-lg px-4 py-2 my-4;
}
.red { @apply border-red-500/40 bg-red-500/5; }
.orange { @apply border-orange-500/40 bg-orange-500/5; }
.amber { @apply border-amber-500/40 bg-amber-500/5; }
.yellow { @apply border-yellow-500/40 bg-yellow-500/5; }
.lime { @apply border-lime-500/40 bg-lime-500/5; }
.green { @apply border-green-500/40 bg-green-500/5; }
.emerald { @apply border-emerald-500/40 bg-emerald-500/5; }
.teal { @apply border-teal-500/40 bg-teal-500/5; }
.cyan { @apply border-cyan-500/40 bg-cyan-500/5; }
.sky { @apply border-sky-500/40 bg-sky-500/5; }
.blue { @apply border-blue-500/40 bg-blue-500/5; }
.indigo { @apply border-indigo-500/40 bg-indigo-500/5; }
.violet { @apply border-violet-500/40 bg-violet-500/5; }
.purple { @apply border-purple-500/40 bg-purple-500/5; }
.fuchsia { @apply border-fuchsia-500/40 bg-fuchsia-500/5; }
.pink { @apply border-pink-500/40 bg-pink-500/5; }
.rose { @apply border-rose-500/40 bg-rose-500/5; }
</style>
