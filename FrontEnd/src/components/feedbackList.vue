<template>
  <div class="vue-tempalte">
    <h3 class="p-3 text-center">List Of Feedback</h3>
    <table class="table table-striped table-bordered table-hover">
      <thead class="thead-dark">
        <tr>
          <th>Id</th>
          <th>Email</th>
          <th>Name</th>
          <th>Mobile No.</th>
          <th>FeedBack</th>
          <th>Suggestion</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(row, id) in rows" v-bind:Key="id">
          <td>{{ id + 1 }}</td>
          <td>{{ row.email }}</td>
          <td>{{ row.FullName }}</td>
          <td>{{ row.mobileNo }}</td>
          <td>{{ row.feedback }}</td>
          <td>{{ row.suggestions }}</td>
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
