<template style="background-color:black">
  <div class="container-fluid pb-5">

    <div class="container menu">
      <div class="container pt-5">
        <img src="../assets/logo.png" style="height:40px" alt="">
      </div>
      <!----------------------OUR Menu------------------- -->
      <div class="container d-flex justify-content-center b-5" id="menu" style="margin-top:10%">

        <div class="container">
          <div class="row text-cener">
            <div class="col-md-3"></div>
            <div class="col-md-5">
              <form action="" class="form">
                <label for="">
                  <h4 class="fw-bold purple_colour">Comment tu t'appelles </h4>
                </label>
                <input type="text" name="comment" placeholder="Name Here" class="purple_border">
              </form>
            </div>
          </div>
        </div>
      </div>

    
      
    </div>

    <div class="container">
      <div class="container div">

      </div>
    </div>

     <div class="cotainer mr-5 mb-5"  style="position:absolute;bottom:-1%;width:90%">
      <div class="row">
        <div class="col-md-11">
          <nav class="navbar"  >

            <a class="nav-link" id="my_row"><p class="mb-5" style="background-color: none!important; color:#fff"><img
                  src="../assets/Frame.svg" style="height:35px;" alt=""></p></a>
            <form class="form-inline mt-5">

              <p>
                <!-- <ul class="nav-item" id="nav_item" style="position:relative;"> -->
              <ul class="nav-item" id="nav_item">
                <li>
                  <router-link to="menu3" class="nav-link left"><img src="../assets/Vector1.svg" alt="">
                  </router-link>
                </li>
                <li>
                  <router-link to="phone" class="nav-link right"><img src="../assets/Vector.svg" alt=""> </router-link>
                </li>
              </ul>
              </p>
            </form>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "comment",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



.cart {
  margin-top: 40px;
}

.div {
  margin-left: -109px;
}

.navbar {
  margin-top: 7%;
  margin-left: 17%;
}

.ul .li {
  display: inline-block;
  padding-left: 10px;
}

.nav-item li {
  display: inline-block;
  position: relative;
}

.nav-item li {
  background-color: #fff;
}

.nav-item li .right {
  background-color: #5ab9ae;
  border-radius: 8px;
}

.nav-item li .left {
  border-radius: 10px !important;
}

input[type="text"] {
  width: 112%;
  height: 58px;
  border-radius: 9px;
  background-color: #f7f7f7;
  padding-left: 10px;
}

.container-fluid {
  background-color: #f7f7f7;
  height: 100vh;
}

#id {
  margin-bottom: 300px;
}

.btn {
  background-color: #5c41f4;
  border: none;
  color: white;
}

.heading {
  color: #5c41f4;
}

.purple_colour {
  color: #524582;
  font-weight: bold;
}

.purple_border {
  border: 2px solid #524582;
}

::-webkit-input-placeholder {
  color: #524582;
}

:-moz-placeholder {
  /* Upto Firefox 18, Deprecated in Firefox 19  */
  color: #524582;
}

::-moz-placeholder {
  /* Firefox 19+ */
  color: #524582;
}

:-ms-input-placeholder {
  color: #524582;
}

input{
  color: #524582;
}

input:focus {
  border: 2px solid #524582;
  color: #524582;
  outline: none;
  font-weight: 500;
}

#my_row {
  margin-bottom: 20px;
}

#nav_item {
  position: relative;
}

@media only screen and (max-width: 769px) {
  .navbar {
  /* margin-top: 7%; */
  margin-left: 0%;
}

.nav-item{
  /* position: relative; */
  margin-right:50px;
}

}

#check {
background: #000;
}

.check {
background: #000;
}

</style>
