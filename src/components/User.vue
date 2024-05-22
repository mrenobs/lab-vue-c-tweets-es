<script setup>


defineProps({
userData: Object

})

</script>

<template>
          
    <span class="user">
        <span class="name" >{{tweets[0].user.name}}</span>
        <span class="handle">{{tweets[0].user.handle }}</span>
    </span>
    

</template>

<style></style>