import { RouterLink } from 'vue-router';

<template>
  <nav class="bg-white fixed bottom-0 md:bottom-auto w-screen z-10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex-shrink-0">
          <!-- Logo -->
          <div class="h-8 w-auto text-blue-500 text-3xl font-bold font-poppins">
            LOGO
          </div>
        </div>
        <div>
          <div class="hidden md:block">
            <RouterLink to="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Home
            </RouterLink>
            <RouterLink to="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Services
            </RouterLink>
            <RouterLink to="#toolsTechnology"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">Tools &
              Technology</RouterLink>
            <RouterLink to="#"
              class="text-black-500 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium font-poppins">How We
              Work</RouterLink>
          </div>
        </div>
        <div class="hidden md:block">
          <!-- Nav items -->
          <button
            class="px-6 py-3 bg-blue-500 hover:bg-blue-100 text-white hover:text-blue-500 text-xs font-semibold rounded-md font-poppins">
            Action Button
          </button>
        </div>
        <div class="md:hidden pr-4">
          <button @click="open = true">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="30" height="30" fill="currentColor">
              <path d="M3 4H21V6H3V4ZM9 11H21V13H9V11ZM3 18H21V20H3V18Z"></path>
            </svg>
          </button>
        </div>
      </div>
    </div>

    <TransitionRoot as="template" :show="open">
      <Dialog as="div" class="relative z-10" @close="open = false">
        <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0" enter-to="opacity-100"
          leave="ease-in-out duration-500" leave-from="opacity-100" leave-to="opacity-0">
          <div class="fixed inset-0 bg-gray-500 bg-opacity-75 transition-opacity" />
        </TransitionChild>

        <div class="fixed inset-0 overflow-hidden">
          <div class="absolute inset-0 overflow-hidden">
            <div class="pointer-events-none fixed inset-y-0 right-0 flex max-w-full pl-10">
              <TransitionChild as="template" enter="transform transition ease-in-out duration-500 sm:duration-700"
                enter-from="translate-x-full" enter-to="translate-x-0"
                leave="transform transition ease-in-out duration-500 sm:duration-700" leave-from="translate-x-0"
                leave-to="translate-x-full">
                <DialogPanel class="pointer-events-auto relative w-screen max-w-md">
                  <TransitionChild as="template" enter="ease-in-out duration-500" enter-from="opacity-0"
                    enter-to="opacity-100" leave="ease-in-out duration-500" leave-from="opacity-100"
                    leave-to="opacity-0">
                    <div class="absolute left-0 top-0 -ml-8 flex pr-2 pt-4 sm:-ml-10 sm:pr-4">
                      <button type="button"
                        class="relative rounded-md text-gray-300 hover:text-white focus:outline-none focus:ring-2 focus:ring-white"
                        @click="open = false">
                        <span class="absolute -inset-2.5" />
                        <span class="sr-only">Close panel</span>
                        <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                      </button>
                    </div>
                  </TransitionChild>
                  <div class="flex h-full flex-col overflow-y-scroll bg-white py-6 shadow-xl">
                    <div class="px-2 bg-white h-full pt-2 pb-3 space-y-1 sm:px-3 ">
                      <RouterLink to="#"
                        class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">
                        Home</RouterLink>
                      <RouterLink to="#services"
                        class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">
                        Services</RouterLink>
                      <RouterLink to="#toolsTechnology"
                        class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">
                        Tools &
                        Technology</RouterLink>
                      <RouterLink to="#"
                        class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">
                        How We
                        Work</RouterLink>
                      <hr class="border-t border-gray-300 w-full">
                      <div class="py-3">
                        <button
                          class="px-6 py-3 bg-blue-500 text-white text-sm font-semibold rounded-md font-poppins w-full">
                          Action Button
                        </button>
                      </div>
                    </div>
                  </div>
                </DialogPanel>
              </TransitionChild>
            </div>
          </div>
        </div>
      </Dialog>
    </TransitionRoot>

    <!-- Mobile menu button -->
    <!-- <div class="md:hidden h-screen fixed z-50 w-full pr-5">
      <div class="px-2 bg-white h-full pt-2 pb-3 space-y-1 sm:px-3 border-t border-gray-300">
        <RouterLink to="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Home</RouterLink>
        <RouterLink to="#services"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Services</RouterLink>
        <RouterLink to="#toolsTechnology"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">Tools &
          Technology</RouterLink>
        <RouterLink to="#"
          class="text-black-500 hover:text-blue-500 block px-3 py-3 rounded-md text-base font-medium font-poppins">How We
          Work</RouterLink>
          <hr class="border-t border-gray-300 w-full">
        <div class="py-3">
          <button class="px-6 py-3 bg-blue-500 text-white text-sm font-semibold rounded-md font-poppins w-full">
            Action Button
          </button>
        </div>
      </div>
    </div> -->
  </nav>




</template>
<script setup>
import { ref } from 'vue'
import { Dialog, DialogPanel, DialogTitle, TransitionChild, TransitionRoot } from '@headlessui/vue'
import { XMarkIcon } from '@heroicons/vue/24/outline'

const open = ref(true)
</script>