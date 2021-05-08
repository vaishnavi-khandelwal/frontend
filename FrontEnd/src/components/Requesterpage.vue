<template>
  <div class="vue-tempalte">
    <form>
       <div class="social-icons mt-3 mb-5">
            <i class="fa fa-user-circle mb-3"></i>
            <h4>Name</h4>
      </div> 

      <p class="forgot-password text-center mb-1">
        <router-link to="/profile">View Profile</router-link>
      </p>
      <hr style="background-color:black;">
      <p class="forgot-password text-center mb-1">
        <router-link to="/ReqHis">My History</router-link>
      </p>
      <hr style="background-color:black;">
      <p class="forgot-password text-center mb-1">
        <router-link to="/requester">Request Product</router-link>
      </p>
      <hr style="background-color:black;">
      <p class="forgot-password text-center mb-1">
        <a href="#" @click="Logout()">Logout</a>
      </p>
    </form>
  </div>
</template>

<script>

</script>
<style>
p{
  font-weight: 700;
}
</style>