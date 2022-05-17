<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="footer-1 ">
          <div class="logo">
logo
          </div>
          <div class="shop-brand">
brand
          </div>
          <div class="useful">
useful
          </div>
          <div class="subscribe">
subscribe
          </div>
        </div>
      </div>
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
.footer-1{
    display: flex;
    justify-content: space-between;
    height: 40vh;
    padding: 20px 0;
    border-bottom: 1px solid grey;
}
</style>
