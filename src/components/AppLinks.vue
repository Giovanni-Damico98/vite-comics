<script>
export default {
  data() {
    return {
      name: "AppLinks",
    };
  },
};
</script>

<template>
  <nav class="d-flex justify-content-center align-items-center gap-5">
    <a href="#">
      <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
      <span>DIGITAL COMICS</span>
    </a>
    <a href="#">
      <img src="../assets/img/buy-comics-merchandise.png" alt="" />
      <span>DC MERCHANDISE</span>
    </a>
    <a href="#">
      <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
      <span>SUBSCRIPTIONS</span>
    </a>
    <a href="#">
      <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
      <span>COMIC SHOP LOCATION</span>
    </a>
    <a href="#">
      <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
      <span>DC POWER VISA</span>
    </a>
  </nav>
</template>

<style scoped lang="scss">
nav {
  height: 150px;
  background-color: #0282f9;
  img {
    height: 50px;
  }
  span {
    color: white;
    margin-left: 10px;
    font-size: 14px;
  }
}
</style>
