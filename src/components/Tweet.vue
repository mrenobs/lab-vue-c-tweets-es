<script setup>
import Profileimage from './Profileimage.vue';
import User from  './user.vue';
import Timestamp from  './Timestamp.vue';
import Message from './Message.vue'
import Action from './Action.vue';

defineProps({
  tweets: Object

});


</script>

<template>


  <div class="tweet" v-for="tweets in tweets">
    <Profileimage :image="user.image">{{ tweets.user.image }}</Profileimage>

    <div class="body" >

      <div class="top">
        <User :userData="Userdata">{{ tweets.user.name }}</User>
        <Timestamp :time="timeStamp">{{tweets.user.handle }}</Timestamp>
      </div>

      <Message :message="message">{{tweets.message}}</Message>

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


