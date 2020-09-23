<template>
  <div id="home" class="container-fluid p-0 m-0 animate__animated animate__fadeIn">
    <Nav />
    <vue-headful :title="title" />
    <div class="row p-0 m-0 w-100 d-flex flex-md-row flex-column-reverse">
      <div class="col-md-6 col-12 px-5 m-auto">
        <h3 class="heading text-center text-md-left "> Sign Up </h3>
        <div class="col-12 col-md-8 py-5">
          <form method="" @submit.prevent="signup()">
              <div class="form-group">
                <label for="">E-Mail</label>
                <input type="email" class="form-control custom_form_input" name="email" id="email" aria-describedby="emailHelpId" placeholder="Enter your e-mail here">              
              </div>
              <div class="form-group">
                <label for="">Password</label>
                <input type="password" class="form-control custom_form_input" name="password" id="password" placeholder="Minimum 6 characters.">
              </div>
              <button type="submit" class="btn btn-orange px-4 px-md-5 py-2">Sign Up</button>
          </form>        
        </div>
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
  name: 'Home',
  components: {
    Nav
  },
  data() {
    return {
      title: 'Home'
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

  .heading
  {
    font-size: 4.5vw;
  }

  
  .custom_form_input
  {
      border: 0.15em solid #FF7F66;
      border-radius: 15px;
      padding: 1%;
  }

  @media screen and (max-width: 820px) {
    
    .heading
    {
      font-size: 3vh;
      letter-spacing: 1px;
    }
    

  }
</style>