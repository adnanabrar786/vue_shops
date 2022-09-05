<template>
  <div class="container">
    <!-- For demo purpose -->
    <div class="row mb-4">
      <div class="col-lg-6 mx-auto text-center"></div>
    </div>
    <!-- End -->
    <div class="row">
      <div class="col-lg-6 mx-auto">
        <div class="card">
          <div class="card-header shadow-lg border-radius">
            <div class="">
              <!-- Credit card form tabs -->
              <ul role="tablist" class="nav nav-pills rounded nav-fill">
                <li>
                  <span class="name">Payment <br /></span>
                </li>
              </ul>
            </div>
            <!-- End -->
            <hr />
            <div class="">
              <!-- Credit card form tabs -->
              <ul role="tablist" class="nav nav-pills">
                <li class="nav-item">
                  Total <br />
                  <h2 class="name">
                    <h3 class="fw-bold" style="font-weight: bold">50$</h3>
                  </h2>
                </li>
                <li class="nav-item"></li>
                <li
                  class="nav-item float-end"
                  style="position: absolute; right: 5%"
                >
                  <img src="../assets/bx_money.svg" alt="" />
                </li>
              </ul>
            </div>
            <!-- End -->
            <br />
            <div class="">
              <!-- Credit card form tabs -->
              <ul role="tablist" class="nav nav-pills rounded nav-fill">
                <!-- <select name="" id="" class="form-control  mt-2">
                  <option value="" class="form-control">Payment Type</option>
                  <option value="">Payment Type</option>
                 <h4>Options</h4>
                </select> -->
                <div class="input_div">
                  <input type="text" placeholder="Payment Type" />
                  <span>Payment Type</span>
                </div>

                <input
                  type="text"
                  class="form-control p-4 mt-4"
                  placeholder="Promo Code Here"
                />
                <input
                  type="text"
                  class="form-control p-4 mt-4"
                  placeholder="Id Here"
                />

                <span style="width: 100%" class="flavour mt-4"
                  >Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                  Dolore cum iste illo? Minima illo deserunt nobis consequatur
                  quisquam quasi cumque veritatis omnis nesciunt ipsum delectus
                  tenetur, quam, eveniet quo adipisci. Lorem ipsum dolor sit
                  amet, maiores officia blanditiis quae veniam, perferendis
                  mollitia ad, itaque, iusto eius alias quis nostrum.
                  Quae?</span
                >
              </ul>
            </div>
            <!-- End -->

            <div class="pt-1 pr-2 pb-2">
              <!-- Credit card form tabs -->
              <ul role="tablist" class="nav nav-pills rounded nav-fill"></ul>
            </div>
            <!-- End -->
            <div class="pt-2 pr-2 pb-2">
              <!-- Credit card form tabs -->
              <ul role="tablist" class="nav nav-pills rounded nav-fill">
                <li class="nav-item"></li>
                <li class="nav-item"></li>
                <li class="nav-item">
                  <button
                    class="btn btn-success"
                    style="background-color: #524582"
                  >
                    Pay
                  </button>
                </li>
              </ul>
            </div>
            <!-- End -->
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="containee pr-5">
    <div class="container pr-5">
      <div
        class="cotainer mr-5 mb-5"
        style="position: absolute; bottom: -1%; width: 90%"
      >
        <div class="row">
          <div class="col-md-10"></div>
        </div>
      </div>
    </div>
  </div>

  <!-- <div class="cotainer mr-5 mb-5" style="position:relative;bottom:-1%;width:60%;left:18%"> -->
  <!-- <div class="row">
        <div class="col-md-11">
          <nav class="navbar ">

            <a class="nav-link"><p class="mb-5" style="background-color: none!important; color:#fff"><img
                  src="../assets/Frame.svg" style="height:35px;" alt=""></p></a>
            <form class="form-inline mt-5">

              <p>
              <ul class="nav-item" style="position:relative;left:5%">
                <li>
                  <router-link to="verifyDetails" class="nav-link left"><img src="../assets/Vector1.svg" alt="">
                  </router-link>
                </li>
                <li>
                  <router-link to="payment" class="nav-link right"><img src="../assets/Vector.svg" alt=""> </router-link>
                </li>
              </ul>
              </p>
            </form>
          </nav>
        </div>
      </div> -->
  <!-- </div>   -->

  <!-- changes  work start -->

  <!-- arrow -->
  <div class="arrow_row">
    <div class="cart_icon">
      <img src="../assets/commentnew/carticon.png" alt="uparrow" />
      <span>Cart</span>
    </div>
    <div class="order_arrow">
      <router-link to="verifyDetails" class="uparrow">
        <img src="../assets/OrderHome/uparrow.png" alt="uparrow" />
      </router-link>
      <router-link to="payment" class="downarrow">
        <img src="../assets/OrderHome/downarrow.png" alt="uparrow" />
      </router-link>
    </div>
  </div>

  <!-- changes  work end -->
</template>

<script>
export default {
  name: "verifyDetails",
  props: {
    msg: String,
  },
};
</script>
<style>
.name {
  font-weight: bold;
  padding-left: 10px;
}

.flavour {
  font-size: 12px;
  margin-left: 8px;
}

.card-header {
  background: #fff;
  border: none !important;
}

.nav-item li .right {
  background-color: #5ab9ae;
  border-radius: 8px;
}

.nav-item li .right {
  background-color: #5ab9ae;
  border-radius: 8px;
}

.nav-pills .nav-link {
  color: #555;
}

.nav-pills .nav-link.active {
  color: white;
}

input[type="radio"] {
  margin-right: 5px;
}

.bold {
  font-weight: bold;
}

/* CHANGES WORK start */
.input_div {
  display: flex;
  align-items: center;
  background-color: #f4f4f4;
  width: 100%;
  height: 50px;
}

.input_div > input {
  border: none;
  outline: none;
  background-color: #f4f4f4;
  width: 75%;
  margin-left: 5%;
  /* color: #9a9a9a; */
}

.input_div > span {
  color: #524582;
  width: 25%;
}

/* arrow_row */

.arrow_row {
  width: 100%;
  display: flex;
  justify-content: space-around;
  position: relative;
  top: 5vh;
  padding-bottom: 20px;
}

/* cart_icon */

.cart_icon {
  background-color: #01b8ae;
  border-radius: 4px;
  width: 100px;
  height: 40px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

.cart_icon > img {
  width: 25px;
  height: 25px;
}

.cart_icon > span {
  color: #ffffff;
}

/* order_arrow six */
.order_arrow {
  display: flex;
}

.order_arrow > button {
  border: none;
  cursor: pointer;
  box-shadow: 0px 10px 60px rgba(226, 236, 249, 0.5);
}

.order_arrow > .uparrow {
  display: flex;
  background: #ffffff;
  width: 50px;
  height: 40px;
  border-top-left-radius: 6px;
  border-bottom-left-radius: 6px;
  box-shadow: 0px 10px 60px rgba(117, 171, 241, 0.5);
}

.uparrow > img {
  width: 12px;
  height: 10px;
  margin: auto;
}

.order_arrow > .downarrow {
  display: flex;
  background: #01b8ae;
  width: 50px;
  height: 40px;
  border-top-right-radius: 6px;
  border-bottom-right-radius: 6px;
}

.downarrow > img {
  width: 12px;
  height: 10px;
  margin: auto;
}

@media only screen and (max-width: 769px) {
  /* arrow_row */

  /* cart_icon */

  .cart_icon {
    width: 80px;
    height: 30px;
  }

  .cart_icon > img {
    width: 15px;
    height: 15px;
  }

  .cart_icon > span {
    font-size: 13px;
  }

  /* order_arrow */
  .order_arrow > .uparrow {
    width: 40px;
    height: 30px;
  }

  .uparrow > img {
    width: 10px;
    height: 8px;
  }

  .order_arrow > .downarrow {
    width: 40px;
    height: 30px;
  }

  .uparrow > img {
    width: 10px;
    height: 8px;
  }
}

@media only screen and (max-width: 600px) {
  .input_div > input {
    width: 70%;
    margin-left: 5%;
  }

  .input_div > span {
    /* color: #524582; */
    width: 30%;
    font-size: 15px;
  }
}

@media only screen and (max-width: 410px) {
  .input_div > input {
    /* width: 70%;
  margin-left: 5%; */
    width: 65%;
  }

  .input_div > span {
    /* color: #524582; */
    /* width: 30%;
  font-size: 15px;
  background: #000; */
    width: 35%;
    font-size: 13px;
  }
}

@media only screen and (max-width: 330px) {
  .input_div > span {
    font-size: 12.5px;
  }
}

/* CHANGES WORK */
</style>
