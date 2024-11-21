<template>
  <div class="login-container">
    <form class="login-form" @submit.prevent="handleSubmit">
      <h2>Login</h2>
      <div class="input-group">
        <label for="email">Email</label>
        <input type="email" v-model="email" id="email" name="email" required />
      </div>
      <div class="input-group">
        <label for="password">Password</label>
        <input
          type="password"
          v-model="password"
          id="password"
          name="password"
          required
        />
      </div>
      <button type="submit">Masuk</button>
      <p class="register-link">
        Belum punya akun?
        <router-link to="/register">Daftar di sini</router-link>
      </p>
    </form>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      email: "",
      password: "",
    };
  },
  methods: {
    handleSubmit() {
      axios
        .post("http://127.0.0.1:8000/api/auth/login", {
          email: this.email,
          password: this.password,
        })
        .then((response) => {
          console.log(response.data);
          this.$router.push("/home");
        })
        .catch((error) => {
          console.error(error);
        });
    },
  },
};
</script>

<style scoped>
body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

h2 {
  text-align: center;
  margin-bottom: 10%;
}

.login-container {
  background-color: white;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.login-form {
  display: flex;
  flex-direction: column;
}

.input-group {
  margin-bottom: 15px;
}

.input-group label {
  margin-bottom: 5px;
}

.input-group input {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  width: 100%;
}

button {
  padding: 10px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

.register-link {
  margin-top: 10px;
  text-align: center;
}
</style>
