<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <FormCard />
    <div>
      <Slider />
    </div>
    <div class="formCenter">
      <div id="FormButton">
        <FormButton />
      </div>
      <div id="FormButton">
        <FormLayout />
      </div>     
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import FormCard from "@/components/FormCard.vue";
import Slider from "@/components/Slider.vue";
import FormLayout from "@/components/FormLayout.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    FormCard,
    Slider,
    FormLayout,
  },
};
</script>

<style lang="sass" scoped>
.formCenter
  background-color: #fff
  margin-left: 26.69%
  margin-top: 20px
  border: 2px solid
  height: 400px
  width: 1200px
</style>
