<template>
  <div class="reach-me">
    <h1>Reach Me</h1>
    <p>Get in touch with me through the following channels: wait dont do that shit just send me your lcation</p>
    <ul>
      <li><a href="mailto:your-email@example.com">Email: your-email@example.com</a></li>
      <li><a href="https://twitter.com/your-twitter-handle" target="_blank">Twitter: @your-twitter-handle</a></li>
      <li><a href="https://github.com/your-github-username" target="_blank">GitHub: @your-github-username</a></li>
    </ul>
    <p>Or, you can fill out the contact form below:</p>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name"><br><br>
      <label for="email">Email:</label>
      <input type="email" id="email" name="email"><br><br>
      <label for="message">Message:</label>
      <textarea id="message" name="message"></textarea><br><br>
      <input type="submit" value="Send">
    </form>
  </div>
</template>

<style scoped>
.reach-me {
  text-align: center;
  padding: 20px;
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

li {
  margin-bottom: 10px;
}

a {
  text-decoration: none;
  color: #337ab7;
}

a:hover {
  color: #23527c;
}

form {
  display: flex;
  flex-direction: column;
  align-items: center;
}

label {
  margin-bottom: 10px;
}

input, textarea {
  padding: 10px;
  margin-bottom: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

input[type="submit"] {
  background-color: #4CAF50;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

input[type="submit"]:hover {
  background-color: #3e8e41;
}
</style>