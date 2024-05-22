<style></style>



<script setup>
defineProps({
    user: Object
})


</script>


<template>
 <img
      src= {{tweets[0].user.image}}
      class="profile"
      alt="profile"
    />

</template>