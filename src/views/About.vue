<template>
  <div id="home" class="container-fluid p-0 m-0 animate__animated animate__fadeIn">
    <Nav />
    <vue-headful :title="title" />
    <div class="row p-0 m-0 w-100 d-flex flex-md-row flex-column-reverse">
      <div class="col-md-6 col-12 px-5 m-auto">
        <h3 class="heading text-center text-md-left font-weight-bold"> About </h3>
        <h2 class="text-center text-md-left font-weight-light "> We are a bunch of computer geeks <i class="fas text-orange fa-grin-wink    "></i> </h2>
        <p class="text-center text-md-left">
          <button class="btn mt-5 btn-lg px-md-4 px-5  py-3 mx-auto btn-orange text-dark" type="button"> Get Started </button>
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
  name: 'About',
  components: {
    Nav
  },
  data() {
    return {
      title: 'About'
    }
  }
}
</script>

<style>
  .graphic_home
  {
    max-height: 60vh;
    max-width: 100%;
    width: auto;
    height: auto;
  }

  .btn-orange
  {
    background-color: #FF7F66;
    border-radius: 35px;
  }

  .text-orange
  {
    color: #FF7F66;
  }

  .heading
  {
    font-size: 4.5vw;
  }

  @media screen and (max-width: 820px) {
    
    .heading
    {
      font-size: 3vh;
      letter-spacing: 1px;
    }
    

  }
</style>