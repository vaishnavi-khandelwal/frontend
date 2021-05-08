<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>Donor</h3>

      <div class="form-group">
        <label>Full Name :</label>
        {{ fullName }}
      </div>

      <div class="form-group">
        <label>Email address :</label>
        {{ email }}
      </div>

      <div class="form-group">
        <label>Mobile Number :</label>
        {{ mobile }}
      </div>
      <div class="form-group">
        <label>Address</label>
        {{ address }}
      </div>
      <div class="form-group">
        <label>Offer Product</label>
        <input
          type="text"
          class="form-control form-control-sm"
          v-model="offer"
          required
        />
      </div>
      <div class="form-group">
        <label>Upload Photo</label>
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