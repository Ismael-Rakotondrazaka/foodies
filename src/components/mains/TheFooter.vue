<template>
  <footer class="p-3 py-10 md:p-20 pb-10">
    <div class="flex flex-row flex-wrap justify-between items-center gap-3">
      <TheLogo />
      <!-- <div class="flex flex-row flex-nowrap items-center gap-2">
        <img src="" alt="logo" />
        <span class="text-black text-lg font-bold">Foodies</span>
      </div> -->
      <div>
        <ul class="flex flex-row flex-wrap gap-x-7 gap-y-3">
          <li class=""><a href="#" class="hover:text-red-500">Services</a></li>
          <li class=""><a href="#" class="hover:text-red-500">Menu</a></li>
          <li class="">
            <a href="#" class="hover:text-red-500">Testimonial</a>
          </li>
          <li class=""><a href="#" class="hover:text-red-500">Promo</a></li>
          <li class=""><a href="#" class="hover:text-red-500">Contact</a></li>
        </ul>
      </div>
    </div>
    <hr class="my-5" />
    <div class="flex flex-row flex-wrap justify-between items-center">
      <div>Copyright &copy; 2022 Foodies. All Right Reserved</div>
      <div>
        <ul class="flex flex-row flex-wrap items-center justify-between gap-7">
          <li class=""><a href="#" class="hover:text-red-500">Security</a></li>
          <li class=""><a href="#" class="hover:text-red-500">Privacy</a></li>
          <li class=""><a href="#" class="hover:text-red-500">Terms</a></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import TheLogo from "@/components/commons/TheLogo.vue";

export default {
  name: "TheFooter",

  components: {
    TheLogo,
  },
};
</script>

<style>
</style>