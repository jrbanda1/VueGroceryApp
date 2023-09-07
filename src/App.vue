<script setup></script>

<template>
  <main>
    <h1 class="title"> :) Vue Grocery List :)</h1>
    <form class="newGroceryFrom">
        <input id="newGrocery" 
        autocomplete="off"
        type="text" 
        placeholder="Add an item to your list">
        <button id="addBtn" type ="submit">Add</button>
    </form>
  </main>
  
</template>

<style lang="postcss" scoped>
  main{
    @apply mt-8 flex flex-col justify-center items-center;
    .title{
      @apply m-2 text-6xl font-light tracking-wider text-accent;
    }
  }
  form{
    @apply mt-8 flex focus-within:ring-8 focus-within:ring-accent focus-within:rounded-lg;
    input{
      @apply bg-white text-comment p-2 w-80 text-xl rounded-l-md outline-none;
    }
    button{
      @apply bg-accent text-background p-2 text-2xl font-bold rounded-r-md;
      &:hover{
        @apply bg-purplish;
      }
    }
  }
</style>