<template>
  <div class="vue-tempalte"> 
     <div class="social-icons mt-3 mb-4">
            <i class="fa fa-check-circle"></i>
      </div> 

      <h3 style="padding-bottom:15px">Thank You !!!</h3>
      <p class="forgot-password text-center" style="padding-bottom:25px">
            Your submission has been received.</p>
      
      <hr style="background-color:blue;">
      
      <div class="main">
          <h6>Please Give Us Your Feedback</h6>
           <router-link style="text-decoration: none;" to=" ">
           <button type="submit" class="btn btn-dark btn-x mt-2">No Thanks</button>
           </router-link> 

           <router-link style="text-decoration: none; padding-left:70px;" to="/feedback">
           <button type="submit" class="btn btn-dark btn-x mt-2">Feedback</button>
           </router-link> 
      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>
