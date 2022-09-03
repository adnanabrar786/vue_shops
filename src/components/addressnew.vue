<template>
  <div>
    <!-- time_logo -->
    <div class="time_logo">
      <img src="../assets/logo.png" alt="BiBimcartlogo" />
    </div>

    <!-- add_detail -->
    <div class="add_detail">
      <p>Quelle est votre adresse</p>
      <h6>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Enim quisque ut
        praesent turpis sit in nulla quis tincidunt in eget.
      </h6>
      <input type="email" placeholder="Email here" class="detail_input" />
    </div>

    <!-- arrow -->

    <!-- arrow -->
    <div class="arrow_row">
      <div class="cart_icon">
        <img src="../assets/commentnew/carticon.png" alt="uparrow" />
        <span>Cart</span>
      </div>
      <div class="order_arrow">
        <router-link to="menu3" class="uparrow">
          <img src="../assets/OrderHome/uparrow.png" alt="uparrow" />
        </router-link>
        <router-link to="phone_numbernew" class="downarrow">
          <img src="../assets/OrderHome/downarrow.png" alt="uparrow" />
        </router-link>
      </div>
    </div>
  </div>
</template>


<script >
export default {
  name: "addressnew",
};
</script>

<style scoped>
/* time_logo  */
.time_logo {
  width: 100%;
  height: 15vh;
  display: flex;
  align-items: center;
  padding-left: 55px;
}

.time_logo > img {
  height: 43px;
  cursor: pointer;
}

/* add detail */

.add_detail {
  /* margin-top: 120px; */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
  top: 15vh;
}

.add_detail > p {
  font-size: 30px;
  width: 50%;
  color: #524582;
}

.add_detail > h6 {
  font-size: 18px;
  margin-bottom: 3vh;
  width: 50%;
  color: #524582;
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

.add_detail > input {
  color: #524582;
  border-radius: 8px;
  border: 2px solid #524582;
  width: 50%;
  height: 50px;
  padding-left: 10px;
}

input:focus {
  border: 2px solid #524582;
  color: #524582;
  outline: none;
  font-weight: 500;
}

/* arrow_row */

.arrow_row {
  width: 100%;
  display: flex;
  justify-content: space-around;
  position: relative;
  top: 40.5vh;
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

@media only screen and (max-width: 971px) {
  /* arrow_row */
  .arrow_row {
    top: 35.5vh;
  }
}

@media only screen and (max-width: 769px) {
  /* .product_logo  */
  .time_logo {
    padding-left: 20px;
  }

  .time_logo > img {
    height: 30px;
  }

  /* add detail */

  .add_detail {
    align-items: center;
  }

  .add_detail > p {
    width: 100%;
    font-size: 24px;
    text-align: center;
  }

  .add_detail > h6 {
    width: 80%;
    font-size: 14px;
    text-align: center;
  }

  .add_detail > input {
    width: 80%;
    height: 40px;
  }

  /* arrow_row */

  .arrow_row {
    top: 49vh;
  }

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

@media only screen and (max-width: 480px) {
  .time_logo > img {
    height: 25px;
  }
}


@media only screen and (max-width: 471px) {
  /* arrow_row */
  .arrow_row {
    top: 46vh;
  }
}
</style>