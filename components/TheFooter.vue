<template>
  <div class="mt-auto h-auto relative overflow-hidden" :class="font">
    <footer class="font-heading" :class="bgColor">
      <div class="p-4 text-center border-b border-black" :class="textColor">
        <div class="nav-links">
          <ul class="text-center flex md:flex-row md:gap-10 flex-col gap-4 justify-center mx-auto font-semibold">
          <li>
            Home
          </li>
          <li>
            API
          </li>
          <li>
            Infrastucture
          </li>
          <li>
            Contact Us
          </li>
        </ul>
        </div>
        
      </div>

      <p class="text-center p-5 text-yellow-400">&copy; ARC Industries</p>
    </footer>
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