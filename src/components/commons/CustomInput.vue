<template>
  <input
    :type="data.type"
    :placeholder="data.placeholder"
    class="
      block
      rounded-full
      bg-red-100 bg-opacity-25
      font-semibold
      text-white text-left
      px-4
      py-3
    "
  />
</template>

<script>
export default {
  name: "CustomInput",
  props: ["data"],
};
</script>

<style>
</style>