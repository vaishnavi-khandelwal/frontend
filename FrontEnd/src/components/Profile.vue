<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
    <h3>My Profile</h3>
        <div class="social-icons mt-3">
            <i class="fa fa-user-circle"></i>
        </div> 
        <div class="form-group">
        <label>Full Name</label>
        <input
          type="text"
          class="form-control form-control-sm"
          v-model="Email"
          disabled
        />
      </div>
      <div class="form-group">
        <label>Email Address</label>
        <input
          type="email"
          class="form-control form-control-sm"
          v-model="Email"
          disabled
        />
      </div>
      
          
    <button type="submit" class="btn btn-dark btn-lg btn-block">Edit</button>
  
    </form>
  </div>
  
</template>

<script>
</script>



