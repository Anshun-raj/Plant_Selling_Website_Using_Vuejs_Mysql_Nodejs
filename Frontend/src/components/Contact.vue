<template>
  <div class="contact">
    <h2><span>contact</span> us</h2>
    <div class="contactData">
      <div class="contactDataLeft">
        <form @submit="getData">
          <input type="text" name="name" placeholder="Name" v-model="form.name" />
          <input type="email" name="email" placeholder="Email" v-model="form.email" />
          <input
            type="number"
            placeholder="Mobile"
            min="10"
            name="mobile"
            v-model="form.mobile"
          />
          <input name="msg" placeholder="Message" v-model="form.message" />
          <button type="submit" class="btn3" @click="getData">Submit</button>
        </form>
      </div>
      <div class="contactDataRight">
        <img src="../assets/contact-img.svg" alt="" class="contactImg" />
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Contact",
  data() {
    return {
      form: {
        name: "",
        email: "",
        mobile: "",
        message: "",
      },
    };
  },
  methods: {
  async getData(e) {
      e.preventDefault();
     const res=await axios({
        method: "post",
        url: "https://localhost:3001/api/insert",
        data:{
          name: this.name,
          email: this.email,
          mobolie: this.mobile,
          message: this.message
        }
      })
    },
  },
};
</script>

<style>
.contact {
  height: 92.5vh;
}

.contact h2 {
  text-align: center;
  font-size: 40px;
  background-color: #f9edf2;
  text-transform: capitalize;
  padding: 5px 0;
  margin: 0 80px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.contact span {
  color: #e84393;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.contact .contactData {
  align-items: center;
  justify-content: space-around;
  height: 90%;
  width: 90%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  margin: 0 50px;
}
.contact .contactData .contactDataLeft {
  width: 50%;
  text-align: center;
  box-shadow: 2px 2px 2px 2px #faecec;
}

.contact .contactData .contactDataLeft form {
  display: block;
  line-height: 3.5;
  margin: 20px 0;
}

.contact .contactData .contactDataLeft form input {
  width: 75%;
  height: 4.5vh;
}

.contact .contactData .contactDataLeft form input::placeholder {
  color: rgb(116, 115, 115);
  font-weight: 600;
  padding: 0 5px;
}

.contact .contactData .contactDataLeft form .btn3 {
  padding: 10px 25px;
  font-weight: bold;
  position: relative;
  font-size: 16px;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  background-color: rgb(79, 78, 78);
  border: none;
  color: #fff;
  border-radius: 20px;
  transition: 0.5s all;
  display: block;
  left: 12%;
}

.contact .contactData .contactDataLeft form .btn3:hover {
  background-color: #e84393;
}

.contact .contactData .contactDataRight {
  text-align: center;
  width: 50%;
}
.contact .contactData .contactDataRight .contactImg {
  width: 500px;
}
</style>
