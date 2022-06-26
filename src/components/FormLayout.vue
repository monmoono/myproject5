<template>
  <div class="card-form" id="cardform">
    <div id="buttonform" v-if="showformbutton">
      <div class="card-area-center">
        <h2 class="card-title">This is Exam Question 1 "Button"</h2>
        <div class="card-button">
          <button type="button" class="btn primary">Primary</button>
          <button type="button" class="btn secondary">Secondary</button>
          <button type="button" class="btn success">Success</button>
          <button type="button" class="btn danger">Danger</button>
          <button type="button" class="btn warning">Warning</button>
          <button type="button" class="btn info">Info</button>
          <button type="button" class="btn light">Light</button>
          <button type="button" class="btn dark">Dark</button>
          <button type="button" class="link">Link</button>
        </div>
      </div>
    </div>

    <div id="formlayout" v-if="showform">
      <h2 class="card-title">This is Exam Question 4 "Form"</h2>

      <div class="card-in-form">
        <div class="input-name">
          <h1>First name</h1>
          <input class="name" />
        </div>
        <div class="input-name">
          <h1>Last name</h1>
          <input class="name" />
        </div>
        <div class="input-name">
          <h1>Username</h1>
          <input class="username" />
        </div>
      </div>

      <div class="card-in-form">
        <div class="input-name">
          <h1>City</h1>
          <input class="name" />
        </div>
        <div class="input-name">
          <h1>state</h1>
          <input class="name" />
        </div>
        <div class="input-name">
          <h1>Zip</h1>
          <input class="number" />
        </div>
      </div>

      <div class="button-form">
        <button type="button" class="btn success">Submit form</button>
        <button type="button" class="btn danger" style="margin-left: 20px">
          Reset
        </button>
      </div>
    </div>
    <footer>
      <div class="card-footer">
        <div class="card-text-footer">          
          <div class="card-text">            
            <div class="pagination-center">
              <div class="pagination">
                <h2 class="card-title" style="margin-top: 20px">This is Exam Question 3 "Pagination"</h2>
                <p style="width: 400px;margin-top: 20px;">If you want to see the results of Exam 4, change the Pagination to
            the next page.</p>
                <!-- <router-link to="/">&laquo;</router-link> |
            <router-link to="/FormButton">1</router-link>
            <router-link to="/FormLayout">2</router-link>
            <router-link to="/contract">&raquo;</router-link>             -->
                <button v-on:click="next((showformbutton = true))">&laquo;</button>
                <button v-on:click="next((showformbutton = true))" ref="bt1">1</button>
                <button v-on:click="next((showformbutton = false))" ref="bt2">2</button>
                <button v-on:click="next((showformbutton = false))">&raquo;</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  el: "#cardform",
  data() {
    return {
      showformbutton: true,
      showform: false,
    };
  },
  methods: {
    next() {
      if (this.showformbutton === true) {
        this.showform = false;
      } else {
        this.showform = true;
      }
    },
  },
};
</script>

<style lang="sass" scoped>
#buttonform
   width: 100%

#formlayout
   width: 100%

.card-footer
    //border: 1px solid #eeee
    position: sticky
    // padding: 15px
    // margin: 0px
    // margin-left: 25%
    // margin-right: 30px
    //margin-top: 300px
    // padding-top: 0px
    // margin-bottom: 0px
    // padding-bottom: 0px

.pagination
    display: flex
    width: 1000px
    margin-left: 150px
    

.pagination button
    color: black
    float: left
    padding: 14px 24px
    text-decoration: none
    margin-top: 20px

.pagination button:active  
    background-color: #333
    color: white
    border-radius: 5px

.pagination button:focus  
    background-color: #333
    color: white
    border-radius: 5px

.pagination button:hover:not(.active)
    background-color: #333
    border-radius: 10px
    color: white

.pagination-center
    float: center
    margin-left: 0
</style>
