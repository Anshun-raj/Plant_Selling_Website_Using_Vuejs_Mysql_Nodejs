<template>
  <div class="navbar">
    <div class="navTitle">
      <h2>Flower<span>Fusion.</span></h2>
    </div>
    <div class="navData">
      <router-link to="/" class="link">Home</router-link>
      <router-link to="/about" class="link">About</router-link>
      <router-link to="/product" class="link">Product</router-link>
      <router-link to="/review" class="link">Review</router-link>
      <router-link to="/contact" class="link">Contact</router-link>
    </div>
    <div class="info">
      <div class="icons">
        <a href="#" class="fas fa-heart"></a>
        <a
          href="#"
          class="fas fa-shopping-cart"
          @click="visibility1 = !visibility1"
        ></a>
        <a href="#" class="fas fa-user" @click="visibility = !visibility"></a>
      </div>
      <div class="cart" v-if="visibility1 === true" id="visible">
        <div class="cartData">
          <img src="../assets/img-1.jpg" class="cartPic" />
          <button class="btn">Remove</button>
        </div>
        <div class="cartData">
          <img src="../assets/img-2.jpg" class="cartPic" />
          <button class="btn">Remove</button>
        </div>
        <div class="cartData">
          <img src="../assets/img-3.jpg" class="cartPic" />
          <button class="btn">Remove</button>
        </div>
        <div class="cartData">
          <img src="../assets/img-4.jpg" class="cartPic" />
          <button class="btn">Remove</button>
        </div>
      </div>

      <div class="profile" v-if="visibility === true" id="visible">
        <img src="../assets/myPic.jpg" alt="" class="bio" />
        <h5>Name:<span>Anshu Narayan</span></h5>
        <h5>Profession:<span>Developer</span></h5>
        <button class="btn">Know More</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      visibility: false,
      visibility1: false,
    };
  },
};
</script>

<style>
.navbar {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  height: 7.5vh;
  background-color: rgba(40, 38, 38, 0.5);
  align-items: center;
}
.navbar .navTitle {
  width: 20%;
}

.navbar .navTitle span {
  color: red;
}

.navbar .navTitle h2 {
  color: #fff;
  font-size: 28px;
}

.navbar .navData {
  display: flex;
  flex-direction: row;
  gap: 30px;
}

.navbar .navData .link {
  text-decoration: none;
  color: #fff;
  font-weight: bold;
  font-size: 22px;
}

.navbar .icons a:hover{
  color: #e84393;
}

#visible {
  visibility: visible;
}

.navbar .icons {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 20px;
  font-size: 22px;
}

.navbar .icons a {
  color: #fff;
}

.navbar .profile {
  width: 200px;
  height: 250px;
  position: absolute;
  text-align: center;
  top: 7.5%;
  background-color: rgb(111, 107, 107);
}

.navbar .profile .bio {
  width: 100px;
  border-radius: 50px;
  margin: 10px 0;
}

.navbar .profile h5 {
  font-size: 16px;
  padding: 5px 0;
  font-weight: bold;
  color: #fff;
}

.navbar .profile span {
  color: red;
}

.navbar .profile .btn {
  padding: 7.5px;
  font-weight: bold;
  border-radius: 5px;
  border: none;
  margin: 10px 0;
  font-weight: bold;
  transition: 0.5s;
}

.navbar .profile .btn:hover {
  background-color: red;
  color: #fff;
}

.navbar .cart {
  padding: 0 30px;
  width: 300px;
  right: 14%;
  height: 450px;
  position: absolute;
  text-align: center;
  display: block;
  top: 7.5%;
  background-color: rgb(111, 107, 107);
}

.navbar .cart .cartData {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 30px;
  margin: 10px 0;
  align-items: center;
}

.navbar .cart .cartData .cartPic {
  width: 100px;
  border-radius: 50px;
}

.navbar .cart .cartData .btn {
  padding: 10px 20px;
  height: 6vh;
  font-weight: bold;
  background-color: red;
  border-radius: 5px;
  border: none;
  font-size: 16px;
  color: #fff;
}
</style>
