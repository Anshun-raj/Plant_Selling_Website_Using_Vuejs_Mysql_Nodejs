<template>
  <div class="review">
    <h2>Customer's <span>Review</span></h2>
    <div class="reviewData">
      <div class="reviewCard">
        <div class="socialIcon">
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
        </div>
        <h4>
          Lorem Ipsum Dolor, Sit Amet Consectetur Adipisicing Elit. Sunt Tenetur
          Voluptas Quibusdam Voluptate Aperiam Eligendi, At Velit Enim? Odit
          Quibusdam Possimus Necessitatibus Atque At Quia Ut Omnis, Sunt
          Corrupti! Id!
        </h4>
        <div class="customerInfo">
          <img src="../assets/pic-2.png" alt="" class="reviewImg" />
          <div class="customerName">
            <h3>Sharon Michel</h3>
          </div>
        </div>
      </div>
      <div class="reviewCard">
        <div class="socialIcon">
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
        </div>
        <h4>
          Lorem Ipsum Dolor, Sit Amet Consectetur Adipisicing Elit. Sunt Tenetur
          Voluptas Quibusdam Voluptate Aperiam Eligendi, At Velit Enim? Odit
          Quibusdam Possimus Necessitatibus Atque At Quia Ut Omnis, Sunt
          Corrupti! Id!
        </h4>
        <div class="customerInfo">
          <img src="../assets/pic-1.png" alt="" class="reviewImg" />
          <div class="customerName">
            <h3>Ricky Ponting</h3>
          </div>
        </div>
      </div>
      <div class="reviewCard">
        <div class="socialIcon">
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star"></i>
          <i class="fas fa-star-half"></i>
        </div>
        <h4>
          Lorem Ipsum Dolor, Sit Amet Consectetur Adipisicing Elit. Sunt Tenetur
          Voluptas Quibusdam Voluptate Aperiam Eligendi, At Velit Enim? Odit
          Quibusdam Possimus Necessitatibus Atque At Quia Ut Omnis, Sunt
          Corrupti! Id!
        </h4>
        <div class="customerInfo">
          <img src="../assets/pic-3.png" alt="" class="reviewImg" />
          <div class="customerName">
            <h3>Charles Deco</h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Review",
};
</script>

<style>
.review {
  height: 92.5vh;
}

.review h2 {
  text-align: center;
  font-size: 40px;
  background-color: #f9edf2;
  text-transform: capitalize;
  padding: 5px 0;
  margin: 0 80px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.review span {
  color: #e84393;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.review .reviewData {
  align-items: center;
  justify-content: space-around;
  height: 90%;
  width: 90%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 0 50px;
}

.review .reviewData .reviewCard {
  width: 300px;
  height: 350px;
  box-shadow: 2px 2px 2px 2px #bdbcbc;
  text-align: left;
  align-items: center;
  border-radius: 5px;
}

.review .reviewData .reviewCard .socialIcon {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

.review .reviewData .reviewCard .socialIcon i {
  font-size: 24px;
  color: #e84393;
  padding: 15px 10px;
}

.review .reviewData .reviewCard h4 {
  font-size: 16px;
  color: #aaa9a9;
  padding: 15px 10px;
}

.review .reviewData .reviewCard .customerInfo {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  text-align: center;
}

.review .reviewData .reviewCard .customerInfo .customerName h3 {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: 24px;
  color: #e84393;
}

.review .reviewData .reviewCard .customerInfo .reviewImg {
  width: 80px;
  border-radius: 50px;
}
</style>
