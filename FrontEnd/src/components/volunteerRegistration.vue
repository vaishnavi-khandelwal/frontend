<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>Volunteer Registration</h3>

      <div class="form-group">
        <label>Full Name</label>
        <input
          type="text"
          class="form-control form-control-sm"
          v-model="fullName"
          required
        />
      </div>

      <div class="form-group">
        <label>Email address</label>
        <input
          type="email"
          class="form-control form-control-sm"
          v-model="email"
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

      <div class="form-group">
        <label>Mobile Number</label>
        <input
          type="tel"
          class="form-control form-control-sm"
          v-model="mob"
          required
        />
      </div>
      <div class="form-group">
        <label>Address</label>
        <textarea
          class="form-control"
          rows="1"
          id="comment"
          v-model="address"
          required
        ></textarea>
      </div>

      <div class="form-group">
        <label>Upload Photo</label><br />
        Upload id proof (Adhaar/Pan card/driving liences)
        <input
          type="file"
          id="file"
          name="file"
          ref="file"
          v-on:change="handelFileUplaod()"
        />
      </div>

      <button type="submit" class="btn btn-dark btn-lg btn-block">
        Submit
      </button>
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
  height: 104%;
}
</style>