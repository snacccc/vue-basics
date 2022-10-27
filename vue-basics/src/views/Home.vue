<template>
   <div class="home">
      <header class="header">
         This is the home page
      </header>

      <p class="description">
         Hello. Yes, welcome. Honestly, there is nothing else to put here. It's just a home page. I don't even know why you're reading this. Well to be fair, there isn't much else anywhere on this website. So I guess this is normal. Here, have this button.
      </p>
   
      <div class="buttons">
         <button @click="clicked = !clicked" class="btn showButton">
            Button
         </button>

         <p v-if="clicked" class="btnReaction">Wow it's working, you're still here. Have another button.</p>

         <button v-if="clicked" @click="count++" class="btn counterBtn">
            {{ count }}
         </button>

         <p v-if="clicked">This one counts the amount of times you've clicked it.</p>

         <p v-else>Wow, it's a button.</p>

         
      </div>

   </div>
</template>

<script>


   export default {
      data() {
         return {
            count: 0,
            clicked: false,
           
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

   .btn {
      width: 6rem;
      height: 3rem;
      cursor: pointer;
      border: none;
      border-radius: 1rem;
      box-shadow: 0px 8px gray;
   }

   .btn:active {
      transform: translateY(4px);
      box-shadow: 0px 4px gray;
   }

   .buttons {
      display: flex;
      flex-direction: column;
      ;
   }

</style>
