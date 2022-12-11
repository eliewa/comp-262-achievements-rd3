<template>
  <div class="p-3" :class="bgColor" >
    <nav class="container flex justify-between mx-auto" :class="textColor">
      <div class="flex">
        <Icon name="gg:bolt" class="text-5xl text-yellow-400"/>
        <p class="font-semibold md:text-2xl text-xl relative top-3" :class="font">ARC Industries</p>
      </div>
      <ul class="md:flex gap-10 text-lg font-semibold relative top-3 lg:gap-20">
        <li>Home</li>
        <li>API</li>
        <li>Infrastucture</li>
      </ul>
      <div class="md:flex relative top-3 gap-3 text-yellow-400">
        <p>Contact Us</p>
        <p>(403)-123-4567</p>
      </div>
    </nav>
  </div>
</template>

<script setup>
  const props = defineProps ({
    bgColor: {
      type: String,
      default: 'bg-black',
    },

    font: {
      type: String,
      default: 'font-sans',
    },
    
    textColor: {
      type: String,
      default: 'text-white',
    }
  })
</script>