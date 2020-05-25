<template>
    <div class="bg-white">

       
        <div class="h-64 w-58 bg-red-700" :style="{ 'background-image': 'url (' + image + ')' }"> <!-- start header -->
            <div class="py-8">
               <div class="flex flex-col items-center">
                  <h1 class="font-bold text-2xl uppercase text-white">mezo<span class="text-yellow-500">s</span>tore</h1>
                  <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 rounded">HOME</a>
                  <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 rounded">ABOUT</a>
                  <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 rounded">SHOPPING</a>
                  <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 rounded">BLOG</a>
                  <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 rounded">CONTACT</a>
               </div>
            </div>
        </div>   <!-- end header -->

         <div class="px-4 py-12"> <!-- start content -->

            <h1 class="text-teal-600 font-bold text-lg uppercase pl-1">Showing All Products</h1>

            <div class="mt-8">
                <div class="grid grid-cols-2">
                   <div class="relative hover-trigger">
                     <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">

                        <button class="relative py-2 px-10  -mt-10  bg-white border border-grey-100 hover-target">
                          Add to Cart
                        </button>
                   </div>

                    <div>
                     <img class="h-56 w-40 rounded object-cover ml-2" src="../assets/image/header.jpg">
                   </div>
                </div>
            </div>
            
         </div> <!-- end content -->
        
    </div>
</template>


<script>

   
   export default{

    data(){

      return {
        image: 'assets/image/header.jpg'
      }
    }

   }
</script>

