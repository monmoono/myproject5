<template>
  <div class="contact">
    <h1 style="font-size: 32px">This is an contact page</h1>
    <section id="contact-form" class="py-3">
      <div class="container">
        <h1 class="l-heading"><span class="text-primary">Contant</span> Us</h1>
        <p>Please fill out the form below to contant us</p>
        <form action="">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" name="name" id="name" />
          </div>
          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" name="email" id="email" />
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea type="message" name="message" id="message"></textarea>
          </div>
          <button type="submit" class="btn">Submit</button>
        </form>
      </div>
    </section>
  </div>
</template>

<style lang="sass" scoped>
div
  background-color: #FFF
.about
  background-color: #fff
  width: 80%
  display: flex
  align-items: center
  justify-content: center
</style>