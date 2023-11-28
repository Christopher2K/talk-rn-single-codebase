<script setup lang="ts">
import { MotionVariants } from "@vueuse/motion";

const props = defineProps<{ image: string }>();

const animation: MotionVariants = {
  initial: {
    y: -10,
  },
  enter: {
    y: 10,
    transition: {
      repeat: Infinity,
      repeatType: "reverse",
      duration: 2000,
    },
  },
};
</script>

<template>
  <div class="slidev-layout default">
    <div class="flex flex-row h-full gap-11">
      <div class="flex-1 flex flex-col justify-center items-start text-center">
        <slot />
      </div>
      <div class="flex-1" v-motion>
        <img v-motion="animation" class="absolute" :src="props.image" />
      </div>
    </div>
  </div>
</template>
