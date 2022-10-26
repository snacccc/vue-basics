<template>
   <div class="home">
      <header class="header">
         This is the home page
      </header>

      <p class="description">
         Hello. Yes, welcome. Honestly, there is nothing else to put here. It's just a home page. I don't even know why you're reading this. Well to be fair, there isn't much else anywhere on this website. So I guess this is normal. Here is a button to hopefully keep you interested and captivate you to stay on this website for an eternity.
      </p>

      <button @click="count++" class="counterBtn">
         {{ count }}
      </button>

      <p class="btnReaction">Wow it's working, you're still here.</p>

   </div>
</template>

<script>

   export default {
      data() {
         return {
            count: 0
         }
      }
   }
   
</script>

<style scoped>
   .home {
      padding: 1rem;
      margin: 1rem;
   }

   .header {
      font-size: 1.2rem;
   }

   .counterBtn {
      width: 6rem;
      height: 3rem;
      cursor: pointer;
      border: none;
      border-radius: 1rem;
      box-shadow: 0px 8px gray;
   }

   .counterBtn:active {
      transform: translateY(4px);
      box-shadow: 0px 4px gray;
   }

</style>
