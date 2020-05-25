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

         <div class="py-12"> <!-- start content -->

            <h1 class="text-teal-600 font-bold text-2xl uppercase ml-4"> All Products</h1>

            <div class="mt-8">
                <div class="grid grid-cols-2 gap-4">
                  
                       <div class="relative hover-trigger ml-5">
                       <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">

                          <button class="relative py-2  mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                            Add to Cart
                          </button>
                   
                        
                       <div>
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>

                     </div>

                    <div class="relative hover-trigger">
                     <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">
                       
                       <button class="relative py-2 mr-6 mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                          Add to Cart
                        </button>

                         <div class="mr-4">
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>
                   </div>


                       <div class="relative hover-trigger ml-5">
                       <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">

                          <button class="relative py-2  mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                            Add to Cart
                          </button>
                   
                        
                       <div>
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>

                     </div>

                    <div class="relative hover-trigger">
                     <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">
                       
                       <button class="relative py-2 mr-6 mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                          Add to Cart
                        </button>

                         <div class="mr-4">
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>
                   </div>


                       <div class="relative hover-trigger ml-5">
                       <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">

                          <button class="relative py-2  mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                            Add to Cart
                          </button>
                   
                        
                       <div>
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>

                     </div>

                    <div class="relative hover-trigger">
                     <img class="h-56 w-40 rounded object-cover" src="../assets/image/header.jpg">
                       
                       <button class="relative py-2 mr-6 mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
                          Add to Cart
                        </button>

                         <div class="mr-4">
                          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">Women Maroon</h1>

                        <h1 class="text-sm text-gray-900 mt-2 text-center font-bold mx-4"><span class="text-teal-600 line-through mr-2">$975.00</span>$899.99</h1>
                       </div>
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

