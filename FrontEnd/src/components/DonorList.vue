<template>
  <div class="vue-tempalte">
    <h3 class="p-3 text-center">List Of Donor's</h3>
    <table class="table table-striped table-bordered table-hover">
      <thead class="thead-dark">
        <tr>
          <th>Id</th>
          <th>Email</th>
          <th>Name</th>
          <th>Mobile No.</th>
          <th>Address</th>
          <th>Offer</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(row, id) in rows" v-bind:Key="id">
          <td>{{ id + 1 }}</td>
          <td>{{ row.email }}</td>
          <td>{{ row.name }}</td>
          <td>{{ row.mobile }}</td>
          <td>{{ row.address }}</td>
          <td>{{ row.OfferProduct }}</td>
        </tr>
      </tbody>
    </table>
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
  width: 800px;
}
</style>
