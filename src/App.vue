<script>

import Friend from './components/Friend.vue'
import { Friends } from './data/friends.js'

export default {
  components: {
    Friend
  },
  data() {
    return {
      friends: Friends
    }
  }
};
</script>


<template>
  <div class="flex w-full min-h-screen items-center justify-center flex-col">
    <div class="flex flex-col lg:flex-row w-5/6 lg:w-1/2">
      <div class="w-full lg:w-1/3 text-2xl lg:text-7xl">
        友链
      </div>
      <div class="text-2xl lg:h-1/6 flex justify-start items-start lg:w-2/3 flex-col">
        Blogroll
        <div class="text-xl lg:text-2xl mt-2 mb-2 lg:mt-0 lg:mb-0">
          Routes: <a href="https://francie.cc" class="hover:text-neutral-500 dark:hover:text-slate-500">/home</a>, <a class="hover:text-neutral-500 dark:hover:text-slate-500" href="https://github.com/franci-e/blogrolls">如何添加友链</a>
        </div>
        

        </div>
        
      </div>

      <div class="bg-neutral-300 dark:bg-slate-600 horizontal-rule w-full h-1"></div>
      
      <div class="w-5/6 lg:w-1/2 mt-2 place-items-stretch grid grid-cols-1 lg:grid-cols-2 lg:gap-4 ">
        <Friend
          v-for="friend in friends"
          :friendName="friend.name"
          :href="friend.href"
          :desc="friend.desc"
          :logoHref="friend.logo_href"
        />
      </div>
      
    </div>
</template>