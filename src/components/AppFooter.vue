<script>
export default {
  data() {
    return {
      name: "AppFooter",
      footerList: [
        {
          title: "DC Comics",
          subtitle: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },
        { title: "Shop", subtitle: ["Shop DC", "Shop DC Collectibles"] },
        {
          title: "DC",
          subtitle: [
            "Term of use",
            "Privacy policy(New)",
            "AD choice",
            "Advertising",
            "Jobs",
            "Subscription",
            "Talent Workshop",
            "CPSC Certificate",
            "Ratings",
            "Shop Help",
            "Contact us",
          ],
        },
        {
          title: "Sites",
          subtitle: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <section id="top-footer">
      <div class="container d-flex">
        <div class="link-list col-md-8">
          <div class="row">
            <div v-for="(item, index) in footerList" :key="index" class="col">
              <h5>
                {{ item.title }}
              </h5>
              <ul>
                <li v-for="(subitem, i) in item.subtitle" :key="i">
                  <a href="#"> {{ subitem }} </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="logo">
          <img src="../assets/img/dc-logo-bg.png" alt="Logo" />
        </div>
      </div>
    </section>
    <section id="bottom-footer" class="d-flex align-items-center">
      <div
        class="footer-jumbotron container d-flex align-items-center justify-content-between"
      >
        <div class="sign-up col-7">
          <button type="button" class="btn btn-outline-primary text-white">
            SIGN-UP NOW!
          </button>
        </div>
        <div class="icons-footer d-flex align-items-center col-5 gap-3">
          <a href="#" class="fw-bold"> FOLLOW US </a>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt=""
          /></a>
          <a href="#"> <img src="../assets/img/footer-twitter.png" alt="" /></a>
          <a href="#"> <img src="../assets/img/footer-youtube.png" alt="" /></a>
          <a href="#">
            <img src="../assets/img/footer-pinterest.png" alt=""
          /></a>
          <a href="#"
            ><img src="../assets/img/footer-periscope.png" alt=""
          /></a>
        </div>
      </div>
    </section>
  </footer>
</template>

<style scoped lang="scss">
.row {
  --bs-gutter-x: -5.5rem;
}
.logo {
  height: 50%;
  img {
    width: 100%;
    height: 100%;
  }
}
#top-footer {
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
  padding: 20px 0;
}

li {
  a {
    text-decoration: none;
    color: #787878;
  }
}

h5 {
  color: white;
}

ul {
  padding-left: 0;
}

#bottom-footer {
  height: 70px;
  background-color: #2c2c2c;
}

.icons-footer {
  width: 50%;
  a {
    text-decoration: none;
  }
}
</style>
