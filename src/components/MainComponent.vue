<template>
  <main>
    <div class="part1 container">
      <div class="browse-category">
        <div class="title">
          <h2>Browse by category</h2>
          <p>
            Augue purus et, tincidunt condimentum mauris. At nibh rutrum mi in.
            Nisi, vitae interdum eleifend dui, consequat nulla rhoncus dictum.
            Viverra.
          </p>
        </div>
        <div class="cards1">
          <div class="card">
            <img src="../assets/img/product-9.jpg" alt="" />
            <p>Bed (1)</p>
          </div>
          <div class="card">
            <img src="../assets/img/product-3.jpg" alt="" />
            <p>Food (6)</p>
          </div>
          <div class="card">
            <img src="../assets/img/product-2.jpg" alt="" />
            <p>Toys (6)</p>
          </div>
          <div class="card">
            <img src="../assets/img/product-4.jpg" alt="" />
            <p>Trasport (6)</p>
          </div>
        </div>
        <div class="cards2">
          <div class="card">
            <h3>Kibble</h3>
            <p>Dry dog food</p>
            <img src="../assets/img/food-transparent-18.png" alt="" />
            <button>Shop dry food</button>
          </div>
          <div class="card">
            <h3>Moist</h3>
            <p>Canned dog food</p>
            <img src="../assets/img/food-transparent-18.png" alt="" />
            <button>Shop moist food</button>
          </div>
          <div class="card">
            <h3>Frozen</h3>
            <p>Freeze-Dried dog food</p>
            <img src="../assets/img/food-transparent-18.png" alt="" />
            <button>Shop frozen food</button>
          </div>
        </div>
      </div>
      <div class="new-arrivals">
        <section class="section1">
          <p>Find the best animal supplies</p>
          <h2>New arrivals weekly</h2>
          <button>Learn more about us</button>
        </section>
        <section class="section2">
          <div class="text debug">
            <div class="left">
              <p>All-time best sellers</p>
              <h2>Items evryone loves</h2>
            </div>
            <div class="right">
              <button>Vew all products</button>
            </div>
          </div>
          <div class="cards debug">
            <div class="card">
              <img src="../assets/img/product-21.jpg" alt="" />
              <h5>trasport cage</h5>
              <p>$25.00</p>
            </div>
            <div class="card">
              <img src="../assets/img/product-20.jpg" alt="" />
              <h5>Dog leash</h5>
              <p>$25.00</p>
            </div>
            <div class="card">
              <img src="../assets/img/product-16.jpg" alt="" />
              <h5>Animal trasport cage</h5>
              <p>
                <span>$35.00</span>
                $25.00
              </p>
            </div>
            <div class="card">
              <img src="../assets/img/product-11.jpg" alt="" />
              <h5>Colorful cat leash</h5>
              <p>$12.00</p>
            </div>
          </div>
        </section>
      </div>
    </div>
    <div class="users-testimonilas debug">
      <h2>Users testimonials</h2>
      <!-- < -->
      <div class="cards container">
        <div class="card">
          <img src="../assets/img/avatar-3.jpg" alt="">
          <p>
          Auctor est habitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, tincidunt eu. Eu.
       </p>
       <p>Lisa Smith, ThemeFusion</p>

        </div>

        <div class="card">
          <img src="../assets/img/avatar-3.jpg" alt="">
          <p>
          Auctor est habitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, tincidunt eu. Eu.
       </p>
       <p>Lisa Smith, ThemeFusion</p>
        </div>


        <div class="card">
          <img src="../assets/img/avatar-3.jpg" alt="">
          <p>
          Auctor est habitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, tincidunt eu. Eu.
       </p>
       <p>Lisa Smith, ThemeFusion</p>
</div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style lang="scss">
// .part1 {
//   height: 100vh;
// }
.part1 .browse-category {
  //height: 180vh;
}
.part1 .browse-category .title {
  margin: 80px auto;
  text-align: center;
}
.part1 .browse-category p {
  margin: 20px 20%;
  font-weight: 100;
  font-size: 15px;
}
.part1 .browse-category .cards1 {
  display: flex;
}
.part1 .browse-category .card img {
  width: calc(100% / 1);
  background-size: contain;
  padding: 10px;
}
.part1 .browse-category .card {
  text-align: center;
}
.part1 .cards2 {
  display: flex;
  margin: 80px 0;
}
.part1 .cards2 .card {
  background: #2a382a;
  background-image: url(../assets/img/bg-transparent-3.png);
  //background-image: linear-gradient(to bottom, #2a382a ,url(../assets/img/bg-transparent-3.png));
  //background-color: linear-gradient( 180 #2a382a);
  margin: 10px;
  padding: 40px 0;
  display: flex;
  justify-content: center;
  flex-flow: column;
  align-items: center;
}
.part1 .cards2 .card img {
  width: 60%;
}
.part1 .cards2 h3 {
  color: white;
  font-size: 30px;
}
.part1 .cards2 p {
  color: #77ab82;
}
.part1 .cards2 button {
  background-color: #77ab82;
  color: white;
  padding: 10px 15px;
  border-radius: 30px;
  border: 0px;
  font-size: 12px;
  cursor: pointer;
}
.section1 {
  background-image: url(../assets/img/banner-3-2x-scaled.jpg);
  width: 100%;
  background-size: cover;
  height: 400px;
  display: flex;
  flex-flow: column wrap;
  justify-content: space-around;
  align-items: center;
  padding: 50px;
  color: white;
  position: relative;
  z-index: 100;
}
.section1 p {
  text-transform: uppercase;
  position: absolute;
  z-index: 100;
  top: 100px;
}
.section1 h2 {
  position: absolute;
  z-index: 100;
  top: 160px;
  font-size: 40px;
}
.section1 button {
  position: absolute;
  z-index: 100;
  top: 250px;
  padding: 10px 15px;
  border-radius: 30px;
  font-size: 12px;
  border: 0px;
  color: gray;
  cursor: pointer;
}
.section1::after {
  display: block;
  position: absolute;
  top: 0px;
  left: 0px;
  content: "";
  height: 100%;

  background-color: rgba(0, 0, 0, 0.349);
  width: 100%;
}
.section2 {
  height: 400px;
  margin: 70px 0px;
}
.section2 .text {
  display: flex;
  justify-content: space-between;
  height: 100px;
}
.section2 .left p {
  color: #2a382a;
  font-weight: 600;
}
.section2 .left h2 {
  margin: 20px 0;
  font-size: 30px;
}
.section2 .right {
  margin-top: 40px;
}
.section2 .right button {
  background-color: #307940;
  color: white;
  padding: 10px 20px;
  border-radius: 30px;
  border: 0px;
  font-size: 12px;
  cursor: pointer;
}
.section2 .cards {
  display: flex;
  text-align: center;
}
.section2 .cards img {
  width: calc(100% / 1);
  background-size: contain;
  padding: 10px;
}
.section2 .cards h5{
  font-weight: 400;
  font-size: 17px;
}
.section2 .cards p{
  color: gray;
  font-size: 15px;
  margin: 10px 0;
}
.section2 .cards p span{
font-size: 12px;
text-decoration: line-through;
}
.users-testimonilas {
text-align: center;
height: 60vh;
padding-top: 60px;
 background: #042d04;
  background-image: url(../assets/img/bg-transparent-3.png);
  color: white;
}
.users-testimonilas h2{
  margin-bottom: 50px;
}

.users-testimonilas .cards{
  display: flex;
  justify-content: center;
  text-align: center;


}
.users-testimonilas .cards img {
  width: 150px;
  background-size: contain;
  padding: 10px;
  border-radius: 50%;
  margin: 0 auto;
}

</style>
