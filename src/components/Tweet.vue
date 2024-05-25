<script setup>
import Profileimage from './Profileimage.vue';
import User from  './user.vue';
import Timestamp from  './Timestamp.vue';
import Message from './Message.vue'
import Action from './Action.vue';

defineProps({
  tweet: Object

});


</script>

<template>


  <div class="tweet">
    <Profileimage :image="tweet.image"></Profileimage>

    <div class="body" >

      <div class="top">
        <User :userData="tweet.user"></User>
        <Timestamp :time="tweet.timestamp"></Timestamp>
      </div>

      <Message :message="tweet.message"></Message>

      <Action></Action>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>

</template>

<style scoped>
a {
  color: #42b983;
}
</style>


