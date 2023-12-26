<template>
  <div class="about">
    <h2><span>about</span> us</h2>
    <div class="aboutData">
      <div class="aboutDataLeft">
        <video src="../assets/about-vid.mp4" loop autoplay muted></video>
        <h3>best flowers sellers</h3>
      </div>
      <div class="aboutDataRight">
        <h3>why choose us?</h3>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Assumenda
          nam cumque quasi autem blanditiis eaque laboriosam, neque alias sequi!
          Minus voluptatem expedita incidunt amet vel repellendus rem nisi
          minima animi?
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit quo
          illum perferendis sapiente iusto distinctio! Esse maxime laborum vero,
          eligendi, sint impedit nulla fugit fugiat qui harum sapiente natus
          cum.
        </p>
        <a href="#" class="btn2">Learn More</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style>
.about {
  height: 92.5vh;
}

.about h2 {
  text-align: center;
  font-size: 40px;
  text-transform: capitalize;
  background-color: #f9edf2;
  padding: 5px 0;
  margin: 0 80px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.about span {
  color: #e84393;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.about .aboutData {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  height: 80%;
  width: 90%;
}

.about .aboutData .aboutDataLeft {
  width: 45%;
  text-align: center;
  box-shadow: 2px 2px 2px 2px #faecec;
}

.about .aboutData .aboutDataLeft h3 {
  background-color: #fff;
  position: absolute;
  top: 50%;
  left: 5%;
  padding: 15px 70px;
  font-size: 32px;
  text-transform: capitalize;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.about .aboutData .aboutDataLeft video {
  width: 80%;
}

.about .aboutData .aboutDataRight {
  width: 50%;
  text-align: left;
}

.about .aboutData .aboutDataRight h3 {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: 36px;
  text-transform: capitalize;
}

.about .aboutData .aboutDataRight p {
  color: rgb(129, 129, 129);
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  padding: 10px 0;
  margin-bottom: 15px;
}

.about .aboutData .aboutDataRight .btn2 {
  text-decoration: none;
  background-color: rgb(54, 53, 53);
  color: #fff;
  font-weight: bold;
  padding: 10px 30px;
  border-radius: 20px;
  font-size: 18px;
  transition: 0.5s all;
}

.about .aboutData .aboutDataRight .btn2:hover {
  background-color: #e84393;
}
</style>
