<template>
  <div class="register-container">
    <form class="register-form" @submit.prevent="handleSubmit">
      <h2>Pendaftaran</h2>

      <div class="input-group">
        <label for="name">Nama Lengkap</label>
        <input v-model="name" type="text" id="name" name="name" required />
      </div>

      <div class="input-group">
        <label for="email">Email</label>
        <input v-model="email" type="email" id="email" name="email" required />
      </div>

      <div class="input-group">
        <label for="password">Password</label>
        <input
          v-model="password"
          type="password"
          id="password"
          name="password"
          required
        />
      </div>

      <button type="submit">Daftar</button>

      <p class="login-link">
        Sudah punya akun?
        <router-link to="/">Login di sini</router-link>
      </p>
    </form>
  </div>
</template>

<script>
import axios from "axios";

export default {
  data() {
    return {
      name: "",
      email: "",
      password: "",
    };
  },
  methods: {
    handleSubmit() {
      console.log("Form submitted with:", {
        name: this.name,
        email: this.email,
        password: this.password,
      });
      try {
        const response = axios.post("http://127.0.0.1:8000/api/auth/register", {
          name: this.name,
          email: this.email,
          password: this.password,
        });
        alert("Registration successful");
        console.log("Registration successful:", response.data);
      } catch (error) {
        alert("Registration failed");
        console.error("Registration failed:", error.response.data);
      }
    },
  },
};
</script>

<style scoped>
body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
}

h2 {
  text-align: center;
  margin-bottom: 10%;
}

.register-container {
  background-color: #fff;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.register-form {
  display: flex;
  flex-direction: column;
}

.input-group {
  margin-bottom: 15px;
}

.input-group label {
  margin-bottom: 5px;
  font-weight: bold;
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

.login-link {
  margin-top: 15px;
  text-align: center;
}
</style>
