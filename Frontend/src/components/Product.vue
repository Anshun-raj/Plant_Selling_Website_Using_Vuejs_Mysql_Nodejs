<template>
  <div class="product">
    <h2>Our <span>Products</span></h2>
    <div class="productData">
      <div class="productCard">
        <h3>-10%</h3>
        <img src="../assets/img-7.jpg" class="productImg" />
        <div class="icons">
          <a href="#" class="fas fa-heart"></a>
          <a href="#" class="fas fa-cart-plus"></a>
          <a href="#" class="fas fa-share"></a>
        </div>
        <h4>Flower Pot</h4>
        <h5>$17.98<span>$25.99</span></h5>
      </div>
      <div class="productCard">
        <h3>-15%</h3>
        <img src="../assets/img-8.jpg" class="productImg" />
        <div class="icons">
          <a href="#" class="fas fa-heart"></a>
          <a href="#" class="fas fa-cart-plus"></a>
          <a href="#" class="fas fa-share"></a>
        </div>
        <h4>Flower Pot</h4>
        <h5>$13.98<span>$19.99</span></h5>
      </div>
      <div class="productCard">
        <h3>-20%</h3>
        <img src="../assets/img-9.jpg" class="productImg" />
        <div class="icons">
          <a href="#" class="fas fa-heart"></a>
          <a href="#" class="fas fa-cart-plus"></a>
          <a href="#" class="fas fa-share"></a>
        </div>
        <h4>Flower Pot</h4>
        <h5>$27.98<span>$35.99</span></h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
};
</script>

<style>
.product {
  height: 92.5vh;
}

.product h2 {
  text-align: center;
  font-size: 40px;
  background-color: #f9edf2;
  text-transform: capitalize;
  padding: 5px 0;
  margin: 0 80px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.product span {
  color: #e84393;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.product .productData {
  /* text-align: center; */
  align-items: center;
  justify-content: space-around;
  height: 90%;
  width: 90%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 0 50px;
}

.product .productData .productCard {
  width: 350px;
  height: 400px;
  box-shadow: 2px 2px 2px 2px #bdbcbc;
  text-align: center;
  align-items: center;
  border-radius: 5px;
}

.product .productData .productCard h3 {
  position: absolute;
  background-color: #e84393;
  top: 30%;
  padding: 8px 10px;
  color: #fff;
  border-radius: 2px;
  margin: 0 15px;
}

.product .productData .productImg {
  width: 200px;
  margin: 20px 0;
}

.product .productData .productCard .icons {
  background-color: #e84393;
  padding: 15px 0;
  text-align: center;
  transition: 0.5s all;
}

.product .productData .productCard .icons:hover {
  background-color: grey;
}

.product .productData .productCard .icons a {
  color: #ffff;
  padding: 0 30px;
  border-right: 1.5px solid #ffff;
  transition: 0.5s all;
  font-size: 20px;
}
.product .productData .productCard .icons a:hover {
  color: #e84393;
}

.product .productData .productCard h4 {
  padding: 10px 0;
  font-size: 26px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  color: rgb(85, 84, 84);
}

.product .productData .productCard h5 {
  padding: 10px 0;
  font-size: 26px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.product .productData .productCard span {
  font-size: 18px;
  text-decoration: line-through;
  color: grey;
}
</style>
