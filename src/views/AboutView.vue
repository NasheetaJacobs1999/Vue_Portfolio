<template>
  <div class="About">
    <h1>About Us</h1>
    <p>Welcome to our website! This is the about page.</p>
    <img src="../assets/logo.png" alt="Our Logo">
    <p>We are a team of passionate developers, designers, and innovators who are dedicated to creating amazing experiences.</p>
    <h2>Our Mission</h2>
    <p>Our mission is to make the world a better place through technology and innovation. i dont like tis wokr</p>
    <h2>Our Team</h2>
    <ul>
      <li>John Doe - CEO</li>
      <li>Jane Doe - CTO</li>
      <li>Bob Smith - Developer</li>
    </ul>
  </div>
</template>
<script>
export default {
  data() {
    return {
      // Add your data properties here
    }
  },
  methods: {
    // Add your methods here
  }
}
</script>
<style>
.About {
  text-align: center;
  padding: 20px;
}
.About img {
  width: 100px;
  height: 100px;
  margin: 20px;
  border-radius: 50%;
}
.About ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.About li {
  padding: 10px;
  border-bottom: 1px solid #ccc;
}
.About li:last-child {
  border-bottom: none;
}
</style>









