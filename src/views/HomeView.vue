<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <FormCard />
    <div>
      <Slider />
    </div>
    <div id="FormButton" class="tabcontent">
      <FormButton />
    </div>
    <div id="Pagination" class="tabcontent">
      <Pagination />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import FormCard from "@/components/FormCard.vue";
import Slider from "@/components/Slider.vue";
import FormButton from "@/components/FormButton.vue";
import Pagination from "@/components/Pagination.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
    FormCard,
    Slider,
    // FormButton,
    // Pagination,
  },
};
</script>
