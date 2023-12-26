<template>
  <div class="home">
    <div class="homeData">
      <h2>Fresh Flowers</h2>
      <h3>Natural & Beautiful Flowers</h3>
      <h5>
        Lorem, Ipsum Dolor Sit Amet Consectetur Adipisicing Elit. Fugit Eveniet
        Aliquid Accusamus Culpa Adipisci Excepturi, Itaque, Molestiae
        Voluptatem!
      </h5>
      <a href="/product" class="btn1">Shop Now</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style>
.home {
  background: url(../assets/background.png) no-repeat;
  background-position: center;
  background-attachment: fixed;
  background-size: cover;
  height: 92.5vh;
  width: 100%;
}

.home .homeData {
  width: 60%;
  padding: 100px;
}

.home .homeData h2 {
  font-weight: bold;
  font-size: 56px;
  color: rgb(68, 68, 68);
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.home .homeData h3 {
  font-size: 35px;
  font-weight: 600;
  color: #e84393;
}

.home .homeData h5 {
  font-weight: 600;
  color: rgb(143, 141, 141);
  font-size: 24px;
  padding: 20px 0;
}

.home .homeData .btn1 {
  padding: 10px 40px;
  background-color: rgb(68, 68, 68);
  border: none;
  font-weight: 600;
  font-size: 18px;
  border-radius: 20px;
  color: #fff;
  cursor: pointer;
  text-decoration: none;
  transition: 0.5s all;
}

.home .homeData .btn1:hover {
  background-color: #e84393;
}
</style>
