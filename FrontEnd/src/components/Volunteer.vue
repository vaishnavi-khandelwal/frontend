<template>
  <div class="vue-tempalte">
   <div class="profile">
          <div class="row">
            <div class="col-md-6 text-right">
                <i class="fa fa-user-circle mb-3"></i>                  
            </div>
            <div class="col-md-6 mt-4">
                  <h4>Name</h4>
                  <h6 class="forgot-password text-left mt-1 mb-3">
                      <router-link to="/profile">View Profile</router-link>
                  </h6>
            </div>
          </div>
    </div>

    <h5 class="text-center mt-3">Work Assigned to me...</h5>
    <div class="row">
      <div class="col-md-6">
        <h4 class="text-center">Donor</h4>
        <table class="table table-striped table-bordered table-hover">
          <thead class="thead-dark">
            <tr>
              <th>Name</th>
              <th>MobileNo</th>
              <th>Address</th>
              <th>OfferProduct</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="(row, id) in donor" v-bind:Key="id">
              <td>{{ row.name }}</td>
              <td>{{ row.mobile }}</td>
              <td>{{ row.address }}</td>
              <td>{{ row.OfferProduct }}</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="col-md-6">
        <h4 class="text-center">Requester</h4>
        <table class="table table-striped table-bordered table-hover">
          <thead class="thead-dark">
            <tr>
              <th>Name</th>
              <th>MobileNo</th>
              <th>Address</th>
              <th>RequestProduct</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="(row, id) in requester" v-bind:Key="id">
              <td>{{ row.name }}</td>
              <td>{{ row.mobile }}</td>
              <td>{{ row.address }}</td>
              <td>{{ row.RequestProduct }}</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <div class="text-center">
      <p>After Completion of Delivery...</p>
      <input
        type="file"
        id="file"
        name="file"
        ref="file"
        v-on:change="handelFileUplaod()"
      />
    </div>
    <div class="text-center mt-3">
      <button
        type="submit"
        class="btn btn-dark btn-lg"
        @click.prevent="formSubmit"
      >
        Submit
      </button>
    </div>
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
.inner-block {
  width: 1010px;
}
</style>