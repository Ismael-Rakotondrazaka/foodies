<template>
  <header
    class="
      py-4
      px-3
      md:px-20
      flex flex-row flex-nowrap
      justify-between
      items-start
      md:items-center
    "
  >
    <TheLogo />
    <div
      class="
        w-2/3
        md:flex
        flex-col
        md:flex-row
        flex-wrap
        justify-between
        items-center
        gap-x-10 gap-y-3
        hidden
      "
    >
      <nav class="">
        <ul
          class="
            flex flex-col
            md:flex-row
            flex-nowrap
            items-center
            justify-between
            gap-x-7
          "
        >
          <li><a href="#" class="hover:text-red-500">Home</a></li>
          <li><a href="#" class="hover:text-red-500">Services</a></li>
          <li><a href="#" class="hover:text-red-500">Menu</a></li>
          <li><a href="#" class="hover:text-red-500">Contact</a></li>
        </ul>
      </nav>
      <div
        class="
          flex flex:col
          md:flex-row
          items-center
          flex-wrap
          justify-center
          gap-x-5
        "
      >
        <figure class="w-5">
          <svg
            class="w-full"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
          >
            <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
            <path
              d="M500.3 443.7l-119.7-119.7c27.22-40.41 40.65-90.9 33.46-144.7C401.8 87.79 326.8 13.32 235.2 1.723C99.01-15.51-15.51 99.01 1.724 235.2c11.6 91.64 86.08 166.7 177.6 178.9c53.8 7.189 104.3-6.236 144.7-33.46l119.7 119.7c15.62 15.62 40.95 15.62 56.57 0C515.9 484.7 515.9 459.3 500.3 443.7zM79.1 208c0-70.58 57.42-128 128-128s128 57.42 128 128c0 70.58-57.42 128-128 128S79.1 278.6 79.1 208z"
            />
          </svg>
        </figure>

        <figure class="w-5">
          <svg
            class="w-full"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 448 512"
          >
            <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
            <path
              d="M112 112C112 50.14 162.1 0 224 0C285.9 0 336 50.14 336 112V160H400C426.5 160 448 181.5 448 208V416C448 469 405 512 352 512H96C42.98 512 0 469 0 416V208C0 181.5 21.49 160 48 160H112V112zM160 160H288V112C288 76.65 259.3 48 224 48C188.7 48 160 76.65 160 112V160zM136 256C149.3 256 160 245.3 160 232C160 218.7 149.3 208 136 208C122.7 208 112 218.7 112 232C112 245.3 122.7 256 136 256zM312 208C298.7 208 288 218.7 288 232C288 245.3 298.7 256 312 256C325.3 256 336 245.3 336 232C336 218.7 325.3 208 312 208z"
            />
          </svg>
        </figure>
        <CustomButton>Login</CustomButton>
      </div>
    </div>
  </header>
</template>

<script>
import CustomButton from "@/components/commons/CustomButton.vue";
import TheLogo from "@/components/commons/TheLogo.vue";

export default {
  name: "TheHeader",
  components: {
    CustomButton,
    TheLogo,
  },
};
</script>

<style>
</style>