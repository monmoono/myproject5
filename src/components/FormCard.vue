<template>
  <div id="app" class="formcard">
    <section id="wrap-main" class="wrap-main">
      <!-- start left bar -->
      <div class="left-bar">
        <div class="card-area-left">
          <div class="card-title-center">
            <h3>286x180</h3>
          </div>
        </div>
        <div class="card-area">
          <h2 class="card-title">This is Exam Question 6 "Card"</h2>
          <div class="card-text">
            <p style="margin-bottom: 15px">
              And this is Exam Question 2 "Modal".
              <br />If you want to see the results of Question 2, press the
              button.
            </p>
            <button class="btn primary" @click="showModal = true">
              Go to Modal
            </button>
            <transition name="slide" appear>
              <div class="modal-overlay" v-if="(showModal = false)"></div>
            </transition>
            <transition name="slide" appear>
              <div class="modal" v-if="showModal">
                <h1>Modal</h1>
                <p>Result of exam 2 modal</p>
                <button
                  class="btn danger"
                  style="margin-left: 190px"
                  @click="showModal = false"
                >
                  Close
                </button>
                <button
                  class="btn primary"
                  style="margin-left: 10px"
                  @click="showModal = false"
                >
                  Save
                </button>
              </div>
            </transition>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style lang="sass" scoped>
h3  
  font-size: 26px
  position: absolute
  left: 110px
  top: 130px

.modal
  position: absolute
  top: 40%
  left: 30%
  right: 50%
  transform: framslate(-50%,-50%)
  z-index: 99

  width: 100%
  max-width: 400px
  background-color: #FFF
  border-radius: 16px
  padding: 25px

  h1
    text-align: left
    font-size: 32px
    font-weight: 900
    margin-button: 15px

  p
    margin-bottom: 50px
    margin-top: 20px
    text-align: left
</style>

<script>
export default {
  el: "#app",
  data() {
    return {
      showModal: true,
    };
  },
};
</script>
