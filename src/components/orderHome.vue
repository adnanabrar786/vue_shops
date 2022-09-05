<template>
  <div class="OrderHome_wrapper_container">
    <div class="OrderHome_wrapper">
      <!-- product_logo -->
      <div class="product_logo">
        <img src="../assets/OrderHome/BiBimcartlogo.png" alt="BiBimcartlogo" />
      </div>

      <!-- OrderHome_details -->
      <div class="OrderHome_details">
        <div class="bibimCircle">
          <p>BiBimCart</p>
        </div>
        <h3>Au Delice De Seoul</h3>
        <div class="icon_div">
          <img src="../assets/OrderHome/facebooklogo.png" alt="facebooklogo" />
          <img src="../assets/OrderHome/instalogo.png" alt="instalogo" />
          <img src="../assets/OrderHome/whatsapplogo.png" alt="whatsapplogo" />
        </div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Interdum eu
          semper orci magnis dolor nullam. Vitae sed amet tempor mi praesent.
        </p>
        <button class="order_button">Commandez maintenant</button>

        <div class="order_arrow">
          <!-- <button class="uparrow">
            <img src="../assets/OrderHome/uparrow.png" alt="uparrow" />
          </button> -->
          <router-link to="orderhome" class="uparrow">
            <img src="../assets/OrderHome/uparrow.png" alt="uparrow" />
          </router-link>
          <router-link to="timenew" class="downarrow">
            <img src="../assets/OrderHome/downarrow.png" alt="uparrow" />
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OrderHome",
};
</script>

<style lang="css" scoped>
.OrderHome_wrapper_container {
  background-color: #ffffff;
  height: 100vh;
}
.OrderHome_wrapper {
  background-image: url("../assets/OrderHome/bgImage.png");
  background-color: #ffffff;
  height: 90vh;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  background-position-x: left;
  background-position-y: bottom;
  font-family: "Merienda", Helvetica, Arial;
}

/* .product_logo  */
.product_logo {
  width: 100%;
  height: 15vh;
  display: flex;
  align-items: center;
  padding-left: 55px;
}

.product_logo > img {
  height: 43px;
  cursor: pointer;
}

/* OrderHome_details */
.OrderHome_details {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  margin-right: 200px;
  /* background: #000; */
  height: 75vh;
  width: 90%;
}

/* bibimCircle  one*/
.bibimCircle {
  display: flex;
  justify-content: center;
  background-color: #ffffff;
  width: 155px;
  height: 155px;
  border-radius: 50%;
  box-shadow: 0px 10px 60px rgba(255, 255, 255, 0.25);
}

.bibimCircle > p {
  margin: auto;
  font-size: 22.5px;
  font-weight: bold;
}

/* OrderHome_details  two*/

.OrderHome_details > h3 {
  color: #ffffff;
  font-size: 23px;
}

/* logo_div three */
.icon_div {
  display: flex;
  justify-content: space-evenly;
  width: 20%;
}

.icon_div > img {
  cursor: pointer;
  width: 30px;
  height: 30px;
}

/* OrderHome_details four */
.OrderHome_details > p {
  width: 30%;
  text-align: center;
  color: #ffffff;
  line-height: 25px;
}

/* button five */
.order_button {
  cursor: pointer;
  color: #524582;
  background-color: #ffffff;
  border: none;
  border-radius: 10px;
  width: 21%;
  width: 300px;
  height: 55px;
  font-size: 20px;
  font-weight: bold;
}

/* order_arrow six */
.order_arrow {
  display: flex;
  justify-content: right;
  width: 70%;
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

@media only screen and (max-width: 1300px) {
  /* bibimCircle  one*/
  .bibimCircle {
    width: 110px;
    height: 110px;
  }

  .bibimCircle > p {
    font-size: 18px;
  }

  /* OrderHome_details  two*/

  .OrderHome_details > h3 {
    font-size: 20px;
  }

  /* logo_div three */
  .icon_div {
    width: 25%;
  }

  .icon_div > img {
    width: 25px;
    height: 25px;
  }

  /* OrderHome_details four */
  .OrderHome_details > p {
    line-height: normal;
    width: 40%;
  }

  /* button five */
  .order_button {
    font-size: 14px;
  }
}

@media only screen and (max-width: 1024px) {
  /* OrderHome_details */
  .OrderHome_details {
    width: 100%;
  }

  /* OrderHome_details four */
  .OrderHome_details > p {
    width: 50%;
  }

  /* button five */
  .order_button {
    width: 23%;
    font-size: 13px;
  }
}

@media only screen and (max-width: 769px) {
  .OrderHome_wrapper {
    height: 89vh;
  }

  /* .product_logo  */
  .product_logo {
    padding-left: 20px;
  }

  .product_logo > img {
    height: 30px;
  }

  /* OrderHome_details */
  .OrderHome_details {
    height: 80vh;
  }

  /* OrderHome_details four */
  .OrderHome_details > p {
    width: 60%;
  }

  /* bibimCircle  one*/
  .bibimCircle {
    width: 100px;
    height: 100px;
  }

  .bibimCircle > p {
    font-size: 17px;
  }

  /* button five */
  .order_button {
    margin-bottom: 30px;
    width: 24%;
    width: 200px;
    font-size: 13px;
  }

  /* order_arrow six */
  .order_arrow {
    width: 90%;
  }

  /* order_arrow six */
  .order_arrow > .uparrow {
    width: 45px;
    height: 35px;
  }

  .uparrow > img {
    width: 11px;
    height: 8px;
  }

  .order_arrow > .downarrow {
    width: 45px;
    height: 35px;
  }

  .downarrow > img {
    width: 11px;
    height: 8px;
  }
}

@media only screen and (max-width: 480px) {
  .OrderHome_wrapper {
    height: 85vh;
  }

  .product_logo > img {
    height: 25px;
  }

  /* bibimCircle  one*/
  .bibimCircle {
    width: 80px;
    height: 80px;
  }

  .bibimCircle > p {
    font-size: 12px;
  }

  /* OrderHome_details  two*/

  .OrderHome_details > h3 {
    font-size: 18px;
  }

  /* logo_div three */
  .icon_div {
    width: 50%;
  }

  /* OrderHome_details four */
  .OrderHome_details > p {
    width: 90%;
    font-size: 15px;
  }
  /* button five */
  .order_button {
    width: 170px;
    height: 45px;
    font-size: 13px;
    margin-bottom: 70px;
  }
}
</style>