<template>
  <nav class="bg-white">
    <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex-shrink-0">
          <!-- Logo -->
          <div class="h-8 w-auto text-blue-500 text-3xl font-bold font-poppins">
            LOGO
          </div>
        </div>
        <div>
          <div class="hidden md:block">
            <a href="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Home</a>
            <a href="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Services</a>
            <a href="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Tools &
              Technology</a>
            <a href="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">How We
              Work</a>
          </div>
        </div>
        <div class="hidden md:block">
          <!-- Nav items -->
          <button class="px-6 py-3 bg-blue-500 text-white text-xs font-semibold rounded-md font-poppins">
            Get a Quote
          </button>
        </div>
      </div>
    </div>

    <!-- Mobile menu button -->
    <div class="md:hidden">
      <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 border-t border-gray-300">
        <a href="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Home</a>
        <a href="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Services</a>
        <a href="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Tools &
          Technology</a>
        <a href="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">How We
          Work</a>
          <hr class="border-t border-gray-300 w-full">
        <div class="py-3">
          <button class="px-6 py-3 bg-blue-500 text-white text-sm font-semibold rounded-md font-poppins w-full">
            Action Button
          </button>
        </div>
      </div>
    </div>

  </nav>
</template>
