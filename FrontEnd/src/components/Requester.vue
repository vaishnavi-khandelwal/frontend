<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>Requester</h3>

      <div class="form-group">
        <label>Full Name:</label>
        {{ fullName }}
      </div>

      <div class="form-group">
        <label>Email address:</label>
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
      <fieldset class="form-group">
        <legend>Request Product</legend>
        <div>
          <select v-model="selected">
            <option disabled value="Available">Please Select One</option>
            <option v-for="items in products" v-bind:key="items">
              {{ items }}
            </option>
          </select>
        </div>
      </fieldset>

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
  height: 103%;
}
</style>