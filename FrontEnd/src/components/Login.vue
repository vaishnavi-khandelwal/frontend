<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>Login</h3>
      <div class="form-group">
        <label>Username</label>
        <input
          type="email"
          class="form-control form-control-sm"
          v-model="Email"
          required
        />
      </div>

      <div class="form-group">
        <label>Password</label>
        <input
          type="password"
          class="form-control form-control-sm"
          v-model="pass"
          required
        />
      </div>

      <label>Login As</label>
      <div class="select mb-4">
      <select required>
        <option value="">Select an option</option>
        <option value="1">Admin</option>
        <option value="2">Donor</option>
        <option value="3">Requester</option>
        <option value="4">Volunteer</option>
      </select>
      </div>

      <button
        type="submit"
        class="btn btn-dark btn-lg btn-block"
        onclick="clear()"
      >
        Login
      </button>

      <p class="forgot-password text-right mt-1 mb-4">
        <router-link to="/forgot-password">Forgot password ?</router-link>
      </p>
      
      <div class="social-icons">
        <a href="#" class="fa fa-facebook"></a>
        <a href="#" class="fa fa-google ml-4"></a>
      </div>
     
      <p class="forgot-password text-center mt-2 ">
        Have not account yet ?
        <router-link to="/registration">Register</router-link>
      </p>

    </form>
  </div>
</template>

<script>
</script>

<style>
body,
html,
.App,
.vue-tempalte,
.vertical-center {
  width: 100%;
  height: 100%;
}
.fa {
  padding: 10px;
  font-size: 20px;
  width: 60px;
  margin: 5px 3px;
}
.fa:hover,
.emoji:hover {
  opacity: 0.6;
  color: #ffffff;
  text-decoration: none;
}
</style>



