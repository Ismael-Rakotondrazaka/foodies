<template>
  <button
    class="
      rounded-full
      px-6
      py-2
      font-semibold
      active:scale-95
      focus-visible:outline-none
      focus-within:outline-none
      focus:outline-none
      text-white
      bg-slate-800
      hover:bg-slate-900
    "
    type="button"
  >
    <slot />
    <!-- {{ data.text }} -->
  </button>
</template>

<script>
export default {
  name: "CustomButton",
};
</script>

<style>
</style>