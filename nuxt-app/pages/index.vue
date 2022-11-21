<template>
   <div>
    <p>{{msg}}</p>
    <button class=" bg-orange-600 mx-20" @click="increase">increase</button>
    <button class=" bg-green-600 mx-24" @click="decrease">decrease</button>
   </div>
   
</template>
<script  setup = "ts" >
let msg = ref(0)
function increase(){
    msg.value = msg.value+1;
}
function decrease(){
    msg.value = msg.value-1;
}

   </script>