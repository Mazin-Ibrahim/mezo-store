<template>
  <div class="bg-white">


    <div class="h-64 w-58 bg-red-700 md:h-32" :style="{ 'background-image': 'url (' + image + ')' }"> <!-- start header -->
      <div class="py-8">
       <div class="flex flex-col items-center md:flex-row md:justify-between md:px-8">
        <h1 class="font-bold text-2xl uppercase text-white">mezo<span class="text-yellow-500">s</span>tore</h1>
        <div class="md:mr-4">
         <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 md:py-2 rounded text-center block md:inline">HOME</a>
         <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 md:py-2  rounded text-center block md:inline md:mx-2">ABOUT</a>
         <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 md:py-2  rounded text-center block md:inline md:mx-2">SHOPPING</a>
         <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 md:py-2  rounded text-center block md:inline md:mx-2">BLOG</a>
         <a href="" class="text-white text-base font-semibold mt-2 hover:bg-red-500 px-2 md:py-2  rounded text-center block md:inline md:mx-2">CONTACT</a>
       </div>

     </div>
   </div>
 </div>   <!-- end header -->


 <div class="md:flex md:flex-row md:py-8">   <!-- start md:screen content -->

   <div class="py-12 md:w-3/4"> <!-- start content -->

    <h1 class="text-yellow-500 font-bold text-2xl uppercase ml-4 md:px-32"> All Products</h1>

    <div class="mt-8">
      <div class="grid grid-cols-1 px-4 md:grid-cols-3 md:gap-4 md:px-32">

       <div class="relative hover-trigger border pb-4 mt-8 w-full md:w-48" v-for="(product,index) in products">

         <img class="h-56 w-full md:w-48 rounded object-cover"  :src="product.image">

         <button @click="toCart(product)" class="relative py-2  mx-auto px-8 rounded  -mt-12  bg-red-800 text-white hover:bg-red-500 font-semibold hover-target">
          Add to Cart
        </button>


        <div>
          <h1 class="text-sm text-gray-900 mt-4 text-center font-bold mx-4 ">{{product.name}}</h1>

          <h1 class="text-sm text-gray-700 mt-2 text-center font-bold mx-4"><span class="text-red-600 line-through mr-2">$975.00</span>${{product.price}}</h1>
        </div>

      </div>






    </div>
  </div>

</div> <!-- end content -->

<div class="px-4 md:px-1 md:w-1/4 md:mt-8 md:mr-8 md:w-68">
  <div class="bg-gray-200 rounded-lg">
   <div class="px-4 py-6">
     <h1 class="text-2xl text font-semibold font-serif">MY<span class="text-yellow-700"> CART</span></h1>
   </div>

   <div class="px-2 pb-8">
    <div class="bg-white rounded shadow-md">
     <div class="flex flex-row justify-between mt-4 px-4 bg-white py-4 rounded-t shadow-md">
       <h1 class="text-gray-900 font-semibold ">Checkout</h1>
       <h1 class="text-gray-900 font-semibold ">Items</h1>


     </div>

     <div class="py-4 px-2 flex flex-row justify-between items-center border" v-for="(cart,index) in carts">
       <div class="static ">
        <img class="h-16 w-16 rounded" :src="cart.image">
        <h2 class="absolute  text-white font-semibold w-4 h-4 px-0 py-0 bg-gray-900 rounded-full text-xs -mt-16 mg mx-16 pl-1">{{count}}</h2>
      </div>
      <h1 class="text-gray-900 font-semibold text-base md:text-sm">{{cart.name}}</h1>
      <button class="text-gray-900 font-semibold text-2xl" @click="Add()"><Plus/></button>
      <h1 class="text-gray-900 font-semibold text-base md:text-sm">${{cart.price}}</h1>
      <button class="text-gray-900 font-semibold text-2xl" @click="Min()"><Minus/></button>
    </div>






    <div class="py-4 px-2 flex flex-row justify-between items-center border">
     <button class="py-2 px-8 bg-gray-500 text-white text-gray-900 font-semibold hover:bg-gray-800 rounded">Pay</button>
     <h1 class="text-gray-900 font-semibold ">Total ${{total}}</h1>
   </div>
 </div>
</div>
</div>
</div>
</div>




</div>
</template>


<script>

import Plus from '../components/icons/Plus'
import Minus from '../components/icons/Minus'

export default{

  components: {
    Plus,
    Minus 
  },

  data(){

    return {
      products:[
      {
        id:1,
        image:require('../assets/image/5.jpg'),
        price:5,
        name:'Women Maroon'
      },
      {
        id:2,
        image:require('../assets/image/2.jpg'),
        price:4,
        name:'T-shirt'
      },

      {
        id:3,
        image:require('../assets/image/4.jpg'),
        price:3,
        name:'Trousers'
      },

      ],
      carts:[],
      count:1,
      total:0,
      custemTotal:[]


    }


  },



  methods:{

    toCart(product){

       this.carts.push(product);

       this.carts = [...new Set(this.carts)]

          
          
          for(let check=0;check <= this.carts.length; check++){
             
             
            this.custemTotal.push(this.carts[check].price)
             

             this.custemTotal = [...new Set(this.custemTotal)]

             this.total = this.custemTotal.reduce((a,b) => a + b, 0)
          
          }



          },

          Add(){

            this.count++;
       
          },

          Min(){


            if(this.count != 0){
             this.count--;
           }
         },
       },

     }
     </script>

