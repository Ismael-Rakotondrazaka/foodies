<template>
  <div
    class="
      flex flex-row flex-wrap
      items-start
      justify-between
      p-3
      py-16
      text-white
      bg-red-400
      md:p-20 md:pb-0
      gap-7
    "
  >
    <div class="w-full sm:w-2/5">
      <h1 class="text-2xl font-extrabold text-white mb-7">
        Get the best promos order now before they run out!
      </h1>
      <p class="mb-3">
        Get the best promo from us just for you and we always provide the best
        service for you, order now at foodies.
      </p>
      <img src="@/assets/images/illustrations/illustration-food-3.svg" alt="" />
    </div>
    <form action="" class="w-full sm:w-2/5">
      <CustomInput
        :data="{ type: 'date', placeholder: 'Day' }"
        class="w-full mb-4"
      />
      <CustomInput
        :data="{ type: 'text', placeholder: 'Day' }"
        class="w-full mb-4"
      />
      <CustomInput
        :data="{ type: 'number', placeholder: 'Day' }"
        class="w-full mb-4"
      />
      <CustomButton>Booking now</CustomButton>
    </form>
  </div>
</template>

<script>
import CustomInput from "@/components/commons/CustomInput.vue";
import CustomButton from "@/components/commons/CustomButton.vue";
export default {
  components: {
    CustomInput,
    CustomButton,
  },
};
</script>

<style>
</style>