<template>
  <div
    class="
      flex flex-row flex-wrap
      items-center
      justify-between
      gap-5
      p-3
      py-10
      md:p-20
    "
  >
    <div class="w-full sm:w-2/5">
      <h1 class="text-3xl font-bold text-black mb-7">
        Special Food Every Time For You and The Fastest Delivery In Your City
      </h1>
      <p class="text-justify mb-7">
        Be the fastest in delivering your healthy food and with us order your
        best food anytime and anywhere.
      </p>
      <div class="mb-7 flex flex-row gap-x-10 items-center justify-start">
        <CustomButton class="">Get started</CustomButton>
        <button
          class="
            flex flex-row
            items-center
            font-bold
            text-black
            flex-nowrap
            gap-x-3
            px-4
            py-1
            rounded-full
            hover:ring hover:ring-black
          "
        >
          <svg
            class="w-4 box-content ring ring-black rounded-full px-2 py-1"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 384 512"
          >
            <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
            <path
              d="M361 215C375.3 223.8 384 239.3 384 256C384 272.7 375.3 288.2 361 296.1L73.03 472.1C58.21 482 39.66 482.4 24.52 473.9C9.377 465.4 0 449.4 0 432V80C0 62.64 9.377 46.63 24.52 38.13C39.66 29.64 58.21 29.99 73.03 39.04L361 215z"
            />
          </svg>
          <p class="inline">Order process</p>
        </button>
      </div>
      <ul class="flex flex-row flex-wrap items-start justify-evenly">
        <li
          class="
            flex flex-col flex-wrap
            items-center
            justify-center
            w-24
            text-center text-black
            gap-4
          "
        >
          <figure class="w-10">
            <svg
              class="w-full fill-yellow-400"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 576 512"
            >
              <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
              <path
                d="M0 64C0 28.65 28.65 0 64 0H224V128C224 145.7 238.3 160 256 160H384V198.6C310.1 219.5 256 287.4 256 368C256 427.1 285.1 479.3 329.7 511.3C326.6 511.7 323.3 512 320 512H64C28.65 512 0 483.3 0 448V64zM256 128V0L384 128H256zM576 368C576 447.5 511.5 512 432 512C352.5 512 288 447.5 288 368C288 288.5 352.5 224 432 224C511.5 224 576 288.5 576 368zM476.7 324.7L416 385.4L387.3 356.7C381.1 350.4 370.9 350.4 364.7 356.7C358.4 362.9 358.4 373.1 364.7 379.3L404.7 419.3C410.9 425.6 421.1 425.6 427.3 419.3L499.3 347.3C505.6 341.1 505.6 330.9 499.3 324.7C493.1 318.4 482.9 318.4 476.7 324.7H476.7z"
              />
            </svg>
          </figure>
          <p>240 Reviews (4.8)</p>
        </li>
        <li
          class="
            flex flex-col flex-wrap
            items-center
            justify-center
            w-24
            text-center text-black
            gap-4
          "
        >
          <figure class="w-10">
            <svg
              class="w-full fill-sky-500"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 640 512"
            >
              <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
              <path
                d="M0 155.2C0 147.9 2.153 140.8 6.188 134.7L81.75 21.37C90.65 8.021 105.6 0 121.7 0H518.3C534.4 0 549.3 8.021 558.2 21.37L633.8 134.7C637.8 140.8 640 147.9 640 155.2C640 175.5 623.5 192 603.2 192H36.84C16.5 192 .0003 175.5 .0003 155.2H0zM64 224H128V384H320V224H384V464C384 490.5 362.5 512 336 512H112C85.49 512 64 490.5 64 464V224zM512 224H576V480C576 497.7 561.7 512 544 512C526.3 512 512 497.7 512 480V224z"
              />
            </svg>
          </figure>
          <p>2500+ Restaurants</p>
        </li>
        <li
          class="
            flex flex-col flex-wrap
            items-center
            justify-center
            w-24
            text-center text-black
            gap-4
          "
        >
          <figure class="w-10">
            <svg
              class="w-full fill-red-500"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 512 512"
            >
              <!--! Font Awesome Pro 6.1.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. -->
              <path
                d="M176 56C176 42.75 186.7 32 200 32H216C229.3 32 240 42.75 240 56C240 69.25 229.3 80 216 80H200C186.7 80 176 69.25 176 56zM216 104C229.3 104 240 114.7 240 128C240 141.3 229.3 152 216 152H200C186.7 152 176 141.3 176 128C176 114.7 186.7 104 200 104H216zM72 176C85.26 176 96 186.7 96 200C96 213.3 85.26 224 72 224H56C42.75 224 32 213.3 32 200C32 186.7 42.75 176 56 176H72zM.001 283.4C.001 268.3 12.28 256 27.43 256H484.6C499.7 256 512 268.3 512 283.4C512 353.9 467.6 414.1 405.3 437.5L403.5 451.1C401.5 467.1 387.9 480 371.8 480H140.2C124.1 480 110.5 467.1 108.5 451.1L106.7 437.5C44.36 414.1 0 353.9 0 283.4H.001zM224 200C224 186.7 234.7 176 248 176H264C277.3 176 288 186.7 288 200C288 213.3 277.3 224 264 224H248C234.7 224 224 213.3 224 200zM128 200C128 186.7 138.7 176 152 176H168C181.3 176 192 186.7 192 200C192 213.3 181.3 224 168 224H152C138.7 224 128 213.3 128 200zM120 104C133.3 104 144 114.7 144 128C144 141.3 133.3 152 120 152H104C90.75 152 80 141.3 80 128C80 114.7 90.75 104 104 104H120zM320 200C320 186.7 330.7 176 344 176H360C373.3 176 384 186.7 384 200C384 213.3 373.3 224 360 224H344C330.7 224 320 213.3 320 200zM312 104C325.3 104 336 114.7 336 128C336 141.3 325.3 152 312 152H296C282.7 152 272 141.3 272 128C272 114.7 282.7 104 296 104H312zM416 200C416 186.7 426.7 176 440 176H456C469.3 176 480 186.7 480 200C480 213.3 469.3 224 456 224H440C426.7 224 416 213.3 416 200zM408 104C421.3 104 432 114.7 432 128C432 141.3 421.3 152 408 152H392C378.7 152 368 141.3 368 128C368 114.7 378.7 104 392 104H408zM312 32C325.3 32 336 42.75 336 56C336 69.25 325.3 80 312 80H296C282.7 80 272 69.25 272 56C272 42.75 282.7 32 296 32H312z"
              />
            </svg>
          </figure>
          <p>6000+ Food Items</p>
        </li>
      </ul>
    </div>
    <img
      src="@/assets/images/illustrations/illustration-food-4.svg"
      alt=""
      class="object-cover w-full rounded-full sm:w-2/5 max-h-96"
    />
  </div>
</template>

<script>
import CustomButton from "@/components/commons/CustomButton.vue";

export default {
  name: "TheHeroSection",

  components: {
    CustomButton,
  },
};
</script>

<style>
</style>