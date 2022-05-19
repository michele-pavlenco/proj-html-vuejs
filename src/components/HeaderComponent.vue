<template>
  <header>
    <div id="top" class="container">
      <div class="heder-top">
        <div class="logo">
          <img src="../assets/img/dark-pet-logo.png" alt="" />
        </div>
        <div class="serchbar">
          <input type="text" placeholder="Search..." />
        </div>
        <div class="questions">
          <h4>Questions?</h4>
          <p>Call us : 1.800.123.4567</p>
        </div>
        <div class="profile">
          <i class="fa-solid fa-bag-shopping"></i>
          <i class="fa-solid fa-user"></i>
        </div>
      </div>
      <nav>
        <div v-for="(item, index) in navOptions" :key="index">
          <div class="navoptions">
            {{ item.name }}
            <div v-if="item.options">{{ item.options }}</div>
          </div>
        </div>
      </nav>
    </div>
    <div class="jumbotron">
      <div class="jumbotron-top  container">
        <span>
          <i class="fa-solid fa-map"></i>
          <p>Internetional</p>
          Shipping Services
        </span>
        <span>
          <i class="fa-solid fa-clock"></i> See our
          <p>store hours</p>
          and services
        </span>
        <span>
          <i class="fa-solid fa-check"></i> We price match to give you the
          <p>best details</p>
        </span>
      </div>
      <div class="jumbotron-img">
        <div class="jumbotron-text container">
          <p>Find the best animal supplies</p>
          <h2>
            We know animals are a part of your family, let us help take care of
            them.
          </h2>
          <button>Learn more about us</button>
        </div>
      </div>
      <div class="jumbotron-bottom container debug">
        <img src="../assets/img/food-transparent-5.png" alt="pet food" />
        <div class="jumbotron-bottom-text">
          <p>Get &euro;25 OFF youre first purchase of our homemade pat foof!</p>
          <a href="#">Visit the shop</a>
        </div>
      </div>
      <div class="black-jumbotron"></div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      navOptions: [
        {
          id: 1,
          name: "Home",
          optins: ["Home-Alternate"],
        },
        {
          id: 2,
          name: "Shop",
          optins: [
            "Shop no sidebar",
            "Shop single sidebar",
            "Shop dual sidebar",
            "Simple product",
            "Variable product",
          ],
        },
        {
          id: 3,
          name: "About",
        },
        {
          id: 4,
          name: "Blog",
        },
        {
          id: 5,
          name: "Contact",
        },
        {
          id: 6,
          name: "Shop by brand",
          // options:[]
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.heder-top {
  height: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo img {
  height: 30px;
}
.serchbar input {
  background-color: lightgray;
  padding: 4px;
  border: 1px solid lightgray;
  border-radius: 30px;
  width: 200px;
}
.questions {
  display: flex;
}
.questions p {
  color: gray;
}
.profile i {
  margin-left: 10px;
}
nav {
  height: 50px;
  display: flex;
  justify-content: center;
}
.navoptions {
  margin: 14px;
  font-size: 14px;
    cursor: pointer;
  &:hover {
    text-decoration: underline;

  }
}
.jumbotron {
  background-image: url(../assets/img/bg-transparent-3.png);
  background-size: auto;
  height: calc(100vh - 100px);
  width: 100%;
  background-color: #2a382a;
  color: white;
  position: relative;
}

.jumbotron::after {
  display: block;
  position: absolute;
  top: 0px;
  left: 0px;
  content: "";
  height: 100%;

  background-color: rgba(0, 0, 0, 0.349);
  width: 100%;
}
.jumbotron-top {
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 40px;
  widows: 100%;
  font-size: 13px;
  z-index: 100;
  position: relative;

}
.jumbotron i {
  margin: 0px 5px 0px 5px;
}
.jumbotron-top span {
  display: flex;
  font-weight: 10;
  cursor: pointer;
}
.jumbotron-top p {
  font-weight: bold;
  margin: 0px 4px;
}
.jumbotron-img {
  background-image: url(../assets/img/banner-5-2x-scaled.jpg);
  width: 100%;
  height: calc(100vh - 220px);
  background-size: cover;
  display: flex;
  flex-flow: column;
  flex-wrap: wrap;
  justify-content: center;

}
.jumbotron-img p {
  text-transform: uppercase;
  font-weight: bold;
  font-size: 14px;
  position: absolute;
  z-index: 1000;
  top: 23%;
  
}
.jumbotron-img h2 {
  width: 40%;
  font-size: 40px;
  font-weight: 250;
  margin: 30px 0px;
  position: absolute;
  z-index: 1000;
  top: 28%;
}
.jumbotron-img button {
  padding: 10px 15px;
  font-size: 10px;
  border-radius: 30px;
  border: 0px;
  cursor: pointer;
  position: absolute;
  z-index: 1000;
  top: 60%;
}
.jumbotron-bottom {
  display: flex;
  height: 80px;
  width: 100%;
  position: relative;
}
.jumbotron-bottom img {
  height: 60px;
  position: absolute;
  bottom: 0;
  margin-left: 10%;
  z-index: 100;
}
.jumbotron-bottom-text {
  margin-left: 25%;
  position: absolute;
  display: flex;
  margin-top: 25px;
  z-index: 100;
}
.jumbotron-bottom-text a {
  color: grey;
  margin-left: 20px;
}
</style>
