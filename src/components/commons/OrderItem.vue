<template>
  <div style="" class="w-full max-w-md">
    <div class="relative flex flex-col items-center">
      <img
        :src="item.image"
        alt=""
        class="
          absolute
          top-10
          shadow-lg
          rounded-full
          sm:top-5
          z-20
          w-2/5
          max-w-sm
        "
      />
      <div
        class="
          z-10
          flex flex-col flex-wrap
          items-center
          justify-center
          w-full
          p-5
          pt-24
          mt-32
          text-center
          bg-white
          shadow-xl
          rounded-3xl
        "
      >
        <div class="flex flex-row flex-wrap items-center justify-center mb-4">
          <div class="items-center justify-center">
            <img
              v-for="(voter, i) in item.voters"
              :key="i"
              :src="voter"
              alt=""
              class="
                relative
                inline
                object-cover
                w-8
                h-8
                max-w-xs
                rounded-full
                ring-2 ring-pink-300
              "
              :style="{
                left: `-0.${i+2*i}rem`,
                backgroundColor: 'red'
              }"
            />
            <!--   <img
              src="@/assets/images/avatar1.jpg"
              alt=""
              class="
                relative
                inline
                object-cover
                w-8
                h-8
                max-w-xs
                rounded-full
                ring-2 ring-pink-300
              "
            />
            <img
              src="@/assets/images/avatar2.jpg"
              alt=""
              class="
                relative
                inline
                object-cover
                w-8
                h-8
                max-w-xs
                rounded-full
                ring-2 ring-pink-300
                -left-2
              "
            />
            <img
              src="@/assets/images/avatar3.jpg"
              alt=""
              class="
                relative
                inline
                object-cover
                w-8
                h-8
                max-w-xs
                rounded-full
                ring-2 ring-pink-300
                -left-3
              "
            /> -->
          </div>
          <div class="flex flex-row flex-wrap items-center justify-between">
            <img src="@/assets/images/star.svg" alt="" class="mr-2" />
            <p>{{ item.rating }} ({{ reviews }} Reviews)</p>
          </div>
        </div>
        <div class="mb-4">
          <h1 class="text-xl font-bold text-slate-800">{{ item.name }}</h1>
          <p>{{ item.description }}</p>
        </div>
        <div class="mb-4 text-xl text-pink-500">$ {{ item.price }}</div>
        <CustomButton>Buy now</CustomButton>
      </div>
    </div>
  </div>
</template>

<script>
import CustomButton from "@/components/commons/CustomButton.vue";
export default {
  name: "OrderItem",

  components: {
    CustomButton,
  },

  props: {
    item: {
      type: Object,
    },
  },

  computed: {
    reviews() {
      let result = this.item.reviews;
      let revString = result.toString();
      let len = revString.length;
      if (len > 3 && len < 7) {
        result = `${revString.split("").slice(0, -3).join("")}k`;
      } else if (len >= 7) {
        result = `${revString.split("").slice(0, -6).join("")}b`;
      }
      return result;
    },
  },
};
</script>

<style>
</style>