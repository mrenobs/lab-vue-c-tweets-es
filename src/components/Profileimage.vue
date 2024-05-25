<style></style>



<script setup>
defineProps({
    imagen: Object
})


</script>


<template>
 <img
      src= {{imagen.image}}
      class="profile"
      alt="profile"
    />

</template>