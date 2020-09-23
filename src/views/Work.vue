<template>
  <div id="home" class="container-fluid p-0 m-0 animate__animated animate__fadeIn">
    <Nav />
    <vue-headful :title="title" />
    <div class="row p-0 m-0 w-100">
      <div class="col-md-6 col-12 px-5 m-auto">
        <h1 class="display-3 font-weight-bold"> Digital Product Manager </h1>
        <h2 class=" font-weight-light "> Create a unique illustration for your website. </h2>
        <p class="text-center text-md-left">
          <button class="btn mt-5 btn-lg px-4 py-3 mx-auto btn-orange text-dark" type="button"> Get Started </button>
        </p>
      </div>
      <div class="col-md-6 col-12 m-auto p-5 p-md-0 text-center">
        <img src="../assets/images/home.png" class="img-fluid graphic_home">
      </div>
    </div>
  </div>
</template>

<script>

import Nav from '../components/Nav'

export default {
  name: 'Work',
  components: {
    Nav
  },
  data() {
    return {
      title: 'Work'
    }
  }
}
</script>

<style>
  .graphic_home
  {
    max-height: 65vh;
    max-width: 100%;
    width: auto;
    height: auto;
  }

  .btn-orange
  {
    background-color: #FF7F66;
    border-radius: 35px;
  }
</style>