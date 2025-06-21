<template>
  <section class="flex flex-col">
    <header class="flex justify-between items-center gap-20 container">
      <div>
        <img src="/site-logo.png" alt="" class="w-[60px]" />
      </div>
      <div class="py-3 flex flex-1">
        <input
          type="text"
          placeholder="Search for products"
          class="border rounded-full w-full py-2 px-2"
        />
      </div>
      <div class="flex gap-8">
        <div class="flex items-center gap-6">
          <IconPhone class="size-4" />
          <div class="flex flex-col">
            <span>24 Support</span>
            <span>+1 212-334-0212</span>
          </div>
        </div>
        <div class="flex items-center gap-6">
          <span>
            <IconWorld />
          </span>
          <div class="flex flex-col">
            <span>WorldWide</span>
            <span>Free Shipping</span>
          </div>
        </div>
      </div>
    </header>
    <div class="flex justify-between items-center gap-9 bg-blue-50 container py-2">
      <nav class="flex items-center gap-8">
        <div class="flex gap-2 bg-white px-1 pr-4 rounded-full items-center py-1">
          <span class="bg-blue-500 text-white py-1 px-1 rounded-full">
            <IconHamburger />
          </span>
          <span> All Categories </span>
        </div>
        <ul class="flex gap-5">
          <li><a href="#">Promotions</a></li>
          <li><a href="#">Stores</a></li>
          <li><a href="#">Our Contacts</a></li>
          <li><a href="#">Delivery & Return</a></li>
          <li><a href="#">Outlet</a></li>
        </ul>
      </nav>
      <div class="flex items-center gap-7">
        <div>USA</div>
        <div>USD</div>
        <div class="flex gap-4">
          <span class="bg-white py-2 px-2 rounded-full">
            <IconUser />
          </span>
          <span class="bg-white py-2 px-2 rounded-full">
            <IconCompare />
          </span>
          <span class="bg-white py-2 px-2 rounded-full">
            <IconFavourite />
          </span>
        </div>
        <div class="flex items-center">
          <div class="bg-blue-500 text-white py-2 px-2 rounded-full">
            <IconCart class="size-1" />
          </div>
          <span>$0.00</span>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup lang="ts">
import IconPhone from '../icons/IconPhone.vue'
import IconWorld from '../icons/IconWorld.vue'
import IconCart from '../icons/IconCart.vue'
import IconUser from '../icons/IconUser.vue'
import IconFavourite from '../icons/IconFavourite.vue'
import IconCompare from '../icons/IconCompare.vue'
import IconHamburger from '../icons/IconHamburger.vue'
</script>
<style></style>
