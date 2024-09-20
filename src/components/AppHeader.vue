<script>
export default {
  data() {
    return {
      name: "AppHeader",
      navList: [
        { name: "Characters", active: false },
        { name: "Comics", active: true },
        { name: "Movies", active: false },
        { name: "TV", active: false },
        { name: "Games", active: false },
        { name: "Collectibles", active: false },
        { name: "Videos", active: false },
        { name: "Fans", active: false },
        { name: "News", active: false },
        { name: "Shop", active: false },
      ],
    };
  },
  methods: {
    activeIndex(index) {
      this.navList.forEach((item, i) => {
        item.active = i === index;
      });
    },
  },
};
</script>

<template>
  <div class="container d-flex align-items-center justify-content-center my-2">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="DC Logo" />
    </div>
    <nav class="col-10">
      <ul class="nav-menu list-unstyled gap-3 d-flex justify-content-end">
        <li
          v-for="(item, index) in navList"
          :key="index"
          :class="{ active: item.active }"
          @click="activeIndex(index)"
        >
          {{ item.name }}
        </li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
.nav-menu li {
  cursor: pointer;
  padding: 20px 0;
}

li.active {
  color: #0282f9;
  border-bottom: 10px solid #0282f9;
  padding: 15px 0;
}

.logo img {
  height: 70px;
}

header {
  padding: 10px 0;
}
</style>
