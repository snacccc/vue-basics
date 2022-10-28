<template>
   <div class="home">
      <header class="header">
         This is the home page
      </header>

      <p class="description">
         Hello. Yes, welcome. Honestly, there is nothing else to put here. It's just a home page. I don't even know why you're reading this. Well to be fair, there isn't much else anywhere on this website. So I guess this is normal. Here, have this button.
      </p>
   
      <div class="buttons">
         <Button @click="clicked = !clicked">
            Button
         </Button>

         <p v-if="clicked" class="btnReaction">Wow it's working, you're still here. Have another button.</p>

         <Button v-if="clicked" @click="count++">
            {{ count }}
         </Button>

         <p v-if="clicked">This one counts the amount of times you've clicked it.</p>

         <p v-else>Wow, it's a button.</p>

         
      </div>

   </div>
</template>

<script>


   import Button from "../components/Button.vue";

   export default {
    name: "home",
    compontents: {
        Button,
    },
    data() {
        return {
            count: 0,
            clicked: false,
        };
    },
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

   .buttons {
      display: flex;
      flex-direction: column;
      ;
   }

</style>
