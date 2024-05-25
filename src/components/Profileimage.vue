<style></style>



<script setup>
defineProps({
    imagen: String
})


</script>


<template>
 <img
      src= {{imagen.image}}
      class="profile"
      alt="profile"
    />

</template>