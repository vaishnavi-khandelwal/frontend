<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>Registration</h3>

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
      <fieldset class="form-group">
        <legend>Gender</legend>
        <div class="form-check form-check-inline">
          <label class="form-check-label">
            <input
              class="form-check-input"
              type="radio"
              name="inlineRadioOptions"
              v-model="male"
            />
            Male
          </label>
        </div>
        <div class="form-check form-check-inline">
          <label class="form-check-label">
            <input
              class="form-check-input"
              type="radio"
              name="inlineRadioOptions"
              v-model="female"
            />
            Female
          </label>
        </div>
        <div class="form-check form-check-inline">
          <label class="form-check-label">
            <input
              class="form-check-input"
              type="radio"
              name="inlineRadioOptions"
              v-model="other"
            />
            Other
          </label>
        </div>
      </fieldset>

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
      <label>Register As</label>
      <div class="select mb-4">
      <select required>
        <option value="">Select an option</option>
        <option>Donor</option>
        <option>Requester</option>
      </select>
      </div>

      <button type="submit" class="btn btn-dark btn-lg btn-block">
        Register
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
  height: 106%;
}
</style>