<template>
  <nav>
     <div class="topnav">
        <router-link to="/" class="router-link">Home</router-link> |
        <router-link to="/about" class="router-link">About</router-link>
        <router-link to="/contract" class="router-link">Contract</router-link>
      </div>    
  </nav>  
  <router-view />

</template>

<style lang="sass">
@import './src/assets/main.sass'
</style>
