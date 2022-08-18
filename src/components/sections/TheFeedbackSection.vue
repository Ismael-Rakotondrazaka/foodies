<template>
  <div
    class="
      flex flex-col-reverse flex-wrap
      items-center
      justify-between
      p-3
      py-16
      sm:flex-row
      md:p-20
    "
  >
    <img
      src="@/assets/images/illustrations/illustration-food-2.svg"
      alt=""
      class="w-full rounded-full ring-2 ring-pink-500 sm:w-2/5"
    />
    <div class="w-full sm:w-2/5">
      <h1 class="mb-5 text-2xl font-bold text-black">
        What our customers say about foodies
      </h1>
      <div class="flex flex-row flex-wrap items-center gap-5 mb-3">
        <img
          src="@/assets/images/users/avatar-3.jpg"
          alt="O"
          class="rounded-full ring-pink-500 ring-2 w-14"
        />
        <div>
          <h3 class="text-black">Rafflaido Rayu</h3>
          <p>College Student</p>
        </div>
      </div>
      <p class="mb-3 text-justify">
        The burgers are really delicious, the texture of the food is very
        crunchy on the tongue, the tomato sauce is deliciuos according to my
        taste and the melted cheese makes it taste really good.
      </p>
      <div class="flex flex-wrap items-center gap-3 mb-7">
        <img
          v-for="n in 5"
          :key="n"
          src="@/assets/images/star.svg"
          class="inline"
          alt=""
        />
        <p>4.9 (240k Reviews)</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFeedbackSection",
};
</script>

<style>
</style>