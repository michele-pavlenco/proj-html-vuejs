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
   background-image:url(../assets/img/bg-transparent-3.png); 
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
.part1 .cards2 h3{
    color: white;
    font-size: 30px;  
}
.part1 .cards2 p{
    color: #77ab82;
}
.part1 .cards2 button{
    background-color:#77ab82 ;
    color: white;
    padding: 10px 15px;
    border-radius: 30px;
    border:0px ;
    font-size: 12px;
    cursor: pointer;
}
.section1{
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
.section1 p{
    text-transform: uppercase;
    position: absolute;
    z-index: 100;
    top: 100px;
}
.section1 h2{
     position: absolute;
    z-index: 100;
    top: 160px;
    font-size: 40px;
}
.section1 button{
    position: absolute;
    z-index: 100;
    top: 250px;
    padding: 10px 15px;
    border-radius: 30px;
    font-size: 12px;
    border:0px;
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


</style>
