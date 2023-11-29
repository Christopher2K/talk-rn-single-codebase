<style setup lang="ts"></style>

<template>
  <div
    class="slidev-layout default flex flex-col justify-start items-start gap-2"
  >
    <div
      v-if="$slots.header"
      class="flex flex-col justify-start items-start w-full"
    >
      <slot name="header" />
    </div>

    <div class="flex flex-row justify-start items-start w-full flex-1 gap-2">
      <div v-if="$slots.left" class="flex-1">
        <slot name="left" />
      </div>
      <div v-if="$slots.right" class="flex-1">
        <slot name="right" />
      </div>
    </div>

    <div v-if="$slots.footer">
      <slot name="footer" />
    </div>
  </div>
</template>
