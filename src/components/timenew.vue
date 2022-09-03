<template>
  <div class="time_wrapper">
    <!-- time_logo -->
    <div class="time_logo">
      <img src="../assets/logo.png" alt="BiBimcartlogo" />
    </div>

    <!-- add details -->

    <div class="add_detail">
      <div class="add_detail_heading">
        <p>Quand souhaitez-vous commander</p>
        <h6>Choisissez un jour de ramassage</h6>
      </div>

      <div class="detail_input">
        <!-- detail_input_firstdiv -->
        <div class="detail_input_firstdiv">
          <!-- dropdown -->

          <!-- day -->
          <select name="cars" class="day_select">
            <option value="saab" class="day_select_option">Day</option>
            <option value="opel" class="day_select_option">tuesday</option>
            <option value="audi" class="day_select_option">wednesday</option>
            <option value="saab" class="day_select_option">Thursday</option>
            <option value="opel" class="day_select_option">Friday</option>
            <option value="audi" class="day_select_option">Saturday</option>
            <option value="audi" class="day_select_option">Sunday</option>
          </select>

          <!-- time start -->
          <select name="cars" class="timeStart_select">
            <option value="saab" class="timeStart_select_option">00:00</option>
            <option value="opel" class="timeStart_select_option">1</option>
            <option value="audi" class="timeStart_select_option">2</option>
            <option value="saab" class="timeStart_select_option">3</option>
            <option value="opel" class="timeStart_select_option">4</option>
            <option value="audi" class="timeStart_select_option">5</option>
            <option value="audi" class="timeStart_select_option">6</option>
          </select>

          <div class="minuslogo">
            <img src="../assets/timenew/minus.png" alt="minuslogo" />
          </div>

          <!-- time end -->
          <select name="cars" class="timeStart_select">
            <option value="saab" class="timeStart_select_option">00:00</option>
            <option value="opel" class="timeStart_select_option">1</option>
            <option value="audi" class="timeStart_select_option">2</option>
            <option value="saab" class="timeStart_select_option">3</option>
            <option value="opel" class="timeStart_select_option">4</option>
            <option value="audi" class="timeStart_select_option">5</option>
            <option value="audi" class="timeStart_select_option">6</option>
          </select>
          <!-- Am -->
          <select name="cars" class="am_select">
            <option value="saab" class="am_select_option">Am</option>
            <option value="opel" class="am_select_option">Pm</option>
          </select>
          <!-- dropdown -->
        </div>
      </div>
    </div>

    <!-- arrow -->
    <div class="order_arrow">
      <router-link to="orderhome" class="uparrow">
        <img src="../assets/OrderHome/uparrow.png" alt="uparrow" />
      </router-link>
      <router-link to="menu1" class="downarrow">
        <img src="../assets/OrderHome/downarrow.png" alt="uparrow" />
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "timenew",
  //   props: {
  //     msg: String,
  //   },
};
</script>

<style scoped>
.time_wrapper {
  font-family: "Merienda", Helvetica, Arial;
  font-weight: bold;
}

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

/* addd details */

/* add detail */

.add_detail {
  margin-top: 60px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.add_detail_heading {
  text-align: center;
}

.add_detail_heading > p {
  font-size: 30px;
  width: 100%;
  color: #524582;
}

.add_detail_heading > h6 {
  font-size: 20px;
  width: 100%;
  color: #524582;
}

/* select options */

/* detail_input_firstdiv start */
.detail_input_firstdiv {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  margin-top: 60px;
}

/* day_select */
.day_select {
  background-color: #ffffff;
  color: #524582;
  height: auto;
  padding: 5px 0px;
  margin: 0px 5px;
  outline: none;
  font-size: 18px;
  border: 1px solid #524582;
  /* width: 20%; */
  border-radius: 7px;
  cursor: pointer;
  font-weight: bold;
}

/* timeStart_select */
.timeStart_select {
  color: #524582;
  height: auto;
  padding: 5px 0px;
  padding-right: 25px;
  padding-left: 5px;
  margin: 0px 5px;
  /* width: 20%; */
  outline: #ffffff;
  border: 1px solid #524582;
  font-size: 18px;
  border-radius: 7px;
  cursor: pointer;
  font-weight: bold;
}

/* am_select */

.am_select {
  color: #524582;
  height: auto;
  padding: 5px 0px;
  padding-right: 4px;
  margin: 0px 5px;
  /* width: 10%; */
  outline: #ffffff;
  border: 1px solid #524582;
  font-size: 18px;
  border-radius: 7px;
  cursor: pointer;
  font-weight: bold;
}

#top_space {
  margin-top: 20px;
}

/* detail_input_firstdiv end */

/* order_arrow  */
.order_arrow {
  display: flex;
  justify-content: right;
  width: 76.5%;
  margin-top: 204px;
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

@media only screen and (max-width: 1200px) {
  /* order_arrow  */
  .order_arrow {
    margin-top: 179px;
  }

  .add_detail {
    margin-top: 20px;
  }
}

@media only screen and (max-width: 1024px) {
  /* order_arrow  */
  .order_arrow {
    width: 85%;
  }

  .add_detail_heading > p {
    font-size: 25px;
  }

  .add_detail_heading > h6 {
    font-size: 17px;
  }

  /* detail_input_firstdiv start */
  .detail_input_firstdiv {
    margin-top: 30px;
    margin-bottom: 30px;
  }

  /* day_select */
  .day_select {
    font-size: 16px;
  }

  /* timeStart_select */
  .timeStart_select {
    font-size: 16px;
  }

  /* am_select */

  .am_select {
    font-size: 16px;
  }

  /* order_arrow  */
  .order_arrow {
    margin-top: 193px;
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
  /* order_arrow  */
  .order_arrow {
    margin-top: 216px;
    width: 95%;
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

  .add_detail {
    margin-top: 30px;
    width: 100%;
  }

  /* time_logo  */
  .time_logo {
    padding-left: 20px;
  }

  .time_logo > img {
    height: 30px;
  }
}

@media only screen and (max-width: 480px) {

  .time_logo > img {
    height: 25px;
  }

  /* add details */

  .add_detail_heading {
    text-align: center;
    width: 100%;
  }

  .add_detail_heading > p {
    font-size: 20px;
  }

  .add_detail_heading > h6 {
    font-size: 15px;
  }

  /* select options */

  /* day_select */
  .day_select {
    font-size: 12px;
    width: 80px;
  }

  /* timeStart_select */
  .timeStart_select {
    padding: 5px 0px;
    padding-right: 2px;
    padding-left: 2px;
    font-size: 12px;
    width: 70px;
  }

  /* am_select */

  .am_select {
    font-size: 12px;
    width: 50px;
  }

  /* detail_input_firstdiv end */

  /* order_arrow  */
  .order_arrow {
    margin-top: 229px;
  }
}

@media only screen and (max-width: 350px) {
  .add_detail_heading > p {
    font-size: 18px;
  }

  .add_detail_heading > h6 {
    font-size: 16px;
  }
}
</style>
