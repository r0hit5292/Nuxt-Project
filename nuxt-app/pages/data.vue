

<script setup>
const { pending, data: alldata } = useFetch(
  "https://jsonplaceholder.typicode.com/users"
 
);
console.log(alldata)
//console.log(data);
watch(alldata, (newAlldata) => {});
</script>
<template>
  <div>
    <div v-if="pending">Loading...</div> 
    <!-- page will show loading while fetch is in pending state -->
    <div v-else>
      <!-- rendering all the data seperately by using V-for -->
      <div
        v-for="items in alldata"
        :key="items"
        class="
          inline-grid
          grid-cols
          bg-slate-400
          m-2
          p-2
          mx-5
          text-[20px]
          capitalize
        "
      >
        <div class="flex flex-col text-center w-64">
          <span class="text-center">{{ items.name }}</span
          ><span class="text-center">{{ items.username }}</span>
        </div>
      </div>
    </div>
  </div>
</template>