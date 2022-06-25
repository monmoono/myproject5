<template>
  <nav>
    <div class="container">
      <div class="topnav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
        <router-link to="/contract">Contract</router-link>
      </div>
    </div>
  </nav>  
  <router-view />

</template>

<style lang="sass">
@import './src/assets/main.sass'
</style>
