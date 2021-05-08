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

        <div class="row">
          <div class="col-md-6">
            <h3 style="margin-top:40px;">Volunteer</h3>
            <p class="forgot-password text-center mt-4">
              <router-link to="/volunteerRegistration">
              New Registration
              </router-link>
            </p>
            <hr style="background-color:black;">
            <p class="forgot-password text-center mb-3">
              <router-link to="/volunteerlist"> 
              View Volunteer List
              </router-link>
            </p>
          </div>

          <div class="col-md-6">
            <h3>Records</h3>
            <p class="forgot-password text-center mt-2 mb-3">
              <router-link to="/donorlist">View Donor List</router-link>
            </p>
            <hr style="background-color:black;">
            <p class="forgot-password text-center mb-3">
              <router-link to="/requesterlist">View Requester List</router-link>
            </p>
            <hr style="background-color:black;">
            <p class="forgot-password text-center mb-3">
              <router-link to="/dailytransaction">Daily Transactions</router-link>
            </p>
            <hr style="background-color:black;">
            <p class="forgot-password text-center mb-3">
            <router-link to="/feedbacklist">View FeedBack List</router-link>
            </p>
          </div>
    </div>

    <p class="forgot-password text-center">    
      <button type="submit" class="btn btn-dark btn-lg">logout</button>
    </p>
  </div>
</template>

<script>

</script>

<style>
p{
  font-weight: 700;
}
.inner-block {
  width: 700px;
}
</style>



