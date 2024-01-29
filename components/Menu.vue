<!-- components/Menu.vue -->
<template>
    <div class="fixed top-0 z-20 items-center w-full  text-center border rounded shadow-md z-2 bg-b-base dark:bg-p-base p-2 pt-2 text-slate-950 dark:text-white text-xl dark:border-gray-700 shadow-blue-600 ">

       <div class="items-center h-full flex justify-between px-2">
       
        <div class=" dark:text-p-show font-bold text-b-show ">
          
                Gabriel
            
        </div>
        <div class=" gap-5 font-bold list-none flex">
            <li class="flex ">
                <NuxtLink to="https://softwarehouse1coder.vercel.app/" target="_blank" class="p-4 rounded-lg hover:text-p-show text-p-base dark:text-blue-500 dark:hover:text-p-show">
                    Software
                </NuxtLink>

                <NuxtLink to="https://www.linkedin.com/in/gabrielfernandesweb" target="_blank" class="p-4 rounded-lg">
                    <img src="/linkedin.png" class="w-8" alt="linkedIn" srcset="">
                </NuxtLink>
            </li>
        </div>
       </div>
    </div>
  </template>
  
<script setup>

const isOpen = ref(false)

defineShortcuts({
  escape: {
    usingInput: true,
    whenever: [isOpen],
    handler: () => { isOpen.value = false }
    }
  
})

    
</script>

