<template>
  <div
    ref="el"
    :class="[
      'transition-all duration-700 ease-out',
      inView ? visibleClasses : hiddenClasses
    ]"
  >
    <slot />
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const el = ref(null);
const inView = ref(false);

// Classes for animation
const hiddenClasses = "opacity-0 translate-y-5";
const visibleClasses = "opacity-100 translate-y-0";

onMounted(() => {
  const observer = new IntersectionObserver(
    (entries) => {
      inView.value = entries[0].isIntersecting; 
      // NO disconnect → animation happens on every scroll
    },
    { threshold: 0.5 }
  );

  observer.observe(el.value);
});
</script>
