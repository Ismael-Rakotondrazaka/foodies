<template>
  <div class="p-3 py-16 md:p-20">
    <div
      class="
        flex flex-row flex-wrap
        items-center
        justify-between
        gap-2
        pt-3
        mb-7
      "
    >
      <h2 class="text-2xl font-bold text-black">Our best menu</h2>
      <div
        class="
          flex flex-row flex-wrap
          items-center
          justify-between
          gap-x-10 gap-y-5
        "
      >
        <form
          action=""
          @submit.prevent=""
          class="flex flex-row flex-wrap gap-x-5 gap-y-3"
        >
          <label for="breakfast">
            <input
              type="radio"
              name="type"
              class="sr-only peer"
              id="breakfast"
            />
            <div
              class="
                inline-block
                px-6
                py-2
                font-semibold
                bg-gray-200
                rounded-full
                active:scale-95
                hover:cursor-pointer hover:bg-gray-300
                peer-checked:text-white
                peer-checked:bg-slate-800
                peer-checked:hover:bg-slate-900
              "
            >
              Breakfast
            </div>
          </label>
          <label for="lunch">
            <input
              type="radio"
              name="type"
              class="sr-only peer"
              id="lunch"
              checked
            />
            <div
              class="
                inline-block
                px-6
                py-2
                font-semibold
                bg-gray-200
                rounded-full
                active:scale-95
                hover:cursor-pointer hover:bg-gray-300
                peer-checked:text-white
                peer-checked:bg-slate-800
                peer-checked:hover:bg-slate-900
              "
            >
              Lunch
            </div>
          </label>
          <label for="dinner">
            <input type="radio" name="type" class="sr-only peer" id="dinner" />
            <div
              class="
                inline-block
                px-6
                py-2
                font-semibold
                bg-gray-200
                rounded-full
                active:scale-95
                hover:cursor-pointer hover:bg-gray-300
                peer-checked:text-white
                peer-checked:bg-slate-800
                peer-checked:hover:bg-slate-900
              "
            >
              Dinner
            </div>
          </label>
          <label for="dessert">
            <input type="radio" name="type" class="sr-only peer" id="dessert" />
            <div
              class="
                inline-block
                px-6
                py-2
                font-semibold
                bg-gray-200
                rounded-full
                active:scale-95
                hover:cursor-pointer hover:bg-gray-300
                peer-checked:text-white
                peer-checked:bg-slate-800
                peer-checked:hover:bg-slate-900
              "
            >
              Desserts
            </div>
          </label>
        </form>
        <div>
          <button
            class="
              px-4
              py-2
              mr-3
              font-semibold
              bg-gray-200
              rounded-full
              active:scale-95
              hover:cursor-pointer hover:bg-gray-300
            "
          >
            <svg
              class="w-4"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 256 512"
            >
              <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
              <path
                d="M192 448c-8.188 0-16.38-3.125-22.62-9.375l-160-160c-12.5-12.5-12.5-32.75 0-45.25l160-160c12.5-12.5 32.75-12.5 45.25 0s12.5 32.75 0 45.25L77.25 256l137.4 137.4c12.5 12.5 12.5 32.75 0 45.25C208.4 444.9 200.2 448 192 448z"
              />
            </svg>
          </button>
          <button
            class="
              px-4
              py-2
              font-semibold
              text-white
              rounded-full
              active:scale-95
              bg-slate-800
              hover:bg-slate-900
            "
          >
            <svg
              class="w-4 fill-white"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 256 512"
            >
              <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
              <path
                d="M64 448c-8.188 0-16.38-3.125-22.62-9.375c-12.5-12.5-12.5-32.75 0-45.25L178.8 256L41.38 118.6c-12.5-12.5-12.5-32.75 0-45.25s32.75-12.5 45.25 0l160 160c12.5 12.5 12.5 32.75 0 45.25l-160 160C80.38 444.9 72.19 448 64 448z"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>
    <div class="flex flex-row flex-wrap items-start gap-5 justify-evenly">
      <OrderItem v-for="item in menu" :key="item.id" :item="item" class="" />
    </div>
  </div>
</template>

<script>
import OrderItem from "@/components/commons/OrderItem.vue";

import pizza from "@/assets/images/foods/slice-pizza.webp";
import hotdog from "@/assets/images/foods/hotdog.webp";
import cookie from "@/assets/images/foods/chocolate-cookies.webp";
import burger from "@/assets/images/foods/cheese-burger.webp";

import avatar1 from "@/assets/images/users/avatar-1.jpg";
import avatar2 from "@/assets/images/users/avatar-2.jpg";
import avatar3 from "@/assets/images/users/avatar-3.jpg";

export default {
  name: "TheMenuSection",
  components: {
    OrderItem,
  },
  data() {
    return {
      menu: [
        {
          id: 1,
          name: "Pizza smoked cheese",
          image: pizza,
          price: 62.25,
          description: "Spicy cheese sauce",
          reviews: 12000,
          rating: 4.0,
          voters: [avatar1, avatar2, avatar3].sort(() => 0.5 - Math.random()),
        },
        {
          id: 2,
          name: "Hotdog slice",
          image: hotdog,
          price: 32.4,
          description: "Medium gribiche sauce",
          reviews: 18000,
          rating: 4.6,
          voters: [avatar1, avatar2, avatar3].sort(() => 0.5 - Math.random()),
        },
        {
          id: 3,
          name: "Cheese burger",
          image: burger,
          price: 68.35,
          description: "Extra moja sauce",
          reviews: 14000,
          rating: 4.2,
          voters: [avatar1, avatar2, avatar3].sort(() => 0.5 - Math.random()),
        },
        {
          id: 4,
          name: "Chocolate cookie",
          image: cookie,
          price: 20.3,
          description: "Delicious chocolate peds",
          reviews: 16000,
          rating: 4.5,
          voters: [avatar1, avatar2, avatar3].sort(() => 0.5 - Math.random()),
        },
      ],
    };
  },
};
</script>

<style>
</style>