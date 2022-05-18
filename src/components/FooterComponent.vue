<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="footer-1">
          <div class="logo">
            <div class="img">
              <img
                src="../assets/img/mobile-light-pet-logo-2x-200x52.png"
                alt=""
              />
            </div>
            <div class="contacts">
              <p>1234 Avada Avenue Avadaville</p>
              <p>info@your-company.com</p>
              <p>Call us: (1) 234 5678</p>
            </div>
          </div>
          <div class="shop-brand">
            <ul>
              <li>Shop by brand</li>
              <li>Bed</li>
              <li>Food</li>
              <li>Toys</li>
              <li>Transport</li>
            </ul>
          </div>
          <div class="useful">
            <ul>
              <li>Useful links</li>
              <li>My account</li>
              <li>Orders</li>
              <li>Checkout</li>
              <li>Cart</li>
            </ul>
          </div>
          <div class="subscribe">
            <p>Subscribe to our newsletter</p>
            <input type="text" placeholder="Insert your email...*">
            <button>Subscribe</button>
          </div>
        </div>
        <div class="footer-2">
          <div class="else">
            <ul>
              <li>home</li>
              <li>about</li>
              <li>blog</li>
              <li>contact</li>
              <li>Shop</li>
            </ul>
          </div>
          <div class="social">
            <ul>
        <li>  <i class="fa-brands fa-facebook-f"></i></li> 
       <li>    <i class="fa-brands fa-twitter"></i></li>
       <li><i class="fa-brands fa-instagram"></i></li>
       <li><i class="fa-brands fa-youtube"></i></li>
           </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      © Copyright 2012 - 2022 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss">
.footer-top {
  width: 100%;
  height: 60vh;
  background-color: green;
  color: white;
  padding: 40px 0;
}
.footer-1 {
  display: flex;
  justify-content: space-between;
  height: 35vh;
  padding: 20px 0;
  border-bottom: 1px solid grey;
}
.footer-1 .logo {
  line-height: 3rem;
}
.footer-1 .logo img {
  width: 170px;
  height: 40px;
}
.footer-1 .logo .contacts p {
  margin-top: 8px;
  line-height: 1rem;
  font-size: 13px;
}
.footer-1 li:first-child {
  font-size: 20px;
}
.footer-1 li {
  line-height: 2rem;
  list-style-type: none;
  font-size: 15px;
}
.footer-1 .subscribe {
  background-color: rgb(15, 72, 15);
  background-image: url(../assets/img/bg-transparent-3.png);
  height: 200px;
  width: 200px;
  padding: 25px;
  border-radius: 5px;
  input{
    padding: 10px 5px;
    border-radius: 30px;
    border:0px;
    margin: 20px 0px;
    width: 100%;
  }
  button{
    background-color:greenyellow;
   width: 100%;
   padding: 10px 5px;
    border-radius: 30px;
    border:0px;
    cursor:pointer;
    
  }}
  .footer-2{
    display: flex;
    flex-flow: column;
    align-items: center;
    ul{
      display: flex;
      list-style-type: none;
    }
    li{
      padding: 20px;
    }
  }
.footer-bottom{
  background-color: black;
  color: white;
  text-align: center;
  padding:30px
}



</style>
