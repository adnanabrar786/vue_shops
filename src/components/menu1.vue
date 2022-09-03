<template>

  <div class="container mt-5">
    <!-- time_logo -->

    <!-- <div class=""> <img src="../assets/logo.png" style="width:20%" alt=""> </div> -->
        <div class="time_logo"> <img src="../assets/logo.png" alt=""> </div>
  </div>

  <div class='container cont mx-auto mt-0 col-md-10 mt-100'>

    <div class="header">
      <h2><small style="color:#524582">Quant souhaite-vous acheter</small></h2>
      <h4><small style="color:#524582">Quant souhaite-vous acheter</small></h4>
    </div>
    <div class="row" style="justify-content: center">
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="row" style="justify-content: center">
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
      <div class="card col-md-3 mt-100">
        <div class="card-content">
          <div class="card-body p-0">
            <div class="profile"> <img src="../assets/menu1.png"> </div>
            <div class="card-title"></div>
            <div class="card-subtitle">
              <p style="font-size:24px!important;color:black" class="text-left">BiBimBap</p>
              <p class="text-left">{{ description }} </p>
              <p style="text-align: end;">
                <button class="btn " style="background-color:#524582">{{ price }} </button>
              </p>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>




  <p>
  <!-- <ul class="nav-item" style="position:relative; margin-left:35%;margin-top:-80px"> -->
  <ul class="nav-item" id="nav_item">
    <li>
      <router-link to="time" class="nav-link left"><img src="../assets/Vector1.svg" alt="">
      </router-link>
    </li>
    <li>
      <router-link to="menu2" class="nav-link right"><img src="../assets/Vector.svg" alt=""> </router-link>
    </li>
  </ul>
  </p>
</template>

<script>
export default {
  name: "menu1",
  props: {
    msg: String,
  },
  data() {
    return {
      list: null,
      title: null,
      description: null,
      price: null,
    };
  },

  methods: {
    get_product() {
      this.axios.get("https://fakestoreapi.com/products/1").then((res) => {
        console.log(res.data);
        this.list = res.data;
        this.title = this.list.title;
        this.description = this.list.description;
        this.price = this.list.price;
      });
    },
  },
  mounted() {
    this.get_product();
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.cont {
  text-align: center;
  border-radius: 20px;
  margin-bottom: 50px;
}

.title {
  font-size: 25px;
  font-weight: 100;
}

.icon {
  position: relative;
  bottom: 14px;
}

.mt-100 {
  margin-top: 100px;
}

.profile img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}

.card {
  border-radius: 15px;
  margin-left: 30px;
  margin-right: 30px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
}

.card-body {
  position: relative;
  bottom: 78px;
}

.btn {
  text-align: center;
  background-color: #ab47bc;
  border: none;
  color: #fff;
}

.btn:hover {
  -webkit-transform: scale(1.05);
  -ms-transform: scale(1.05);
  transform: scale(1.05);
  color: #fff;
}

.header {
  padding-top: 40px;
}

#nav_item {
  position: relative;
  margin-right: 2%;
  margin-top: 80px;
}

@media only screen and (max-width: 480px) {
  #nav_item {
    margin-right: 25%;
  }
}

/* time_logo  */
.time_logo {
  width: 100%;
  /* height: 15vh; */
  display: flex;
  align-items: center;
  /* padding-left: 55px; */
}

.time_logo > img {
  height: 43px;
  cursor: pointer;
}
</style>
