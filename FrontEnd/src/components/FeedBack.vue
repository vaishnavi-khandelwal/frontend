<template>
  <div class="vue-tempalte">
    <form @submit="formSubmit">
      <h3>{{ type }} Feedback</h3>

      <div class="form-group">
        <label>Full Name</label>
        {{ fullname }}
      </div>

      <div class="form-group">
        <label>Email address</label>
        {{ email }}
      </div>

      <div class="form-group">
        <label>Mobile Number</label>
        {{ mobile }}
      </div>
      <p class="text-center">Tell Us How You Really Feel?</p>

      <div class="row justify-content-center" id="rating-div">
        <div class="col-4">
          <button type="button" @click="rating('great')">
            <span class="emoji"> &#128516;</span>
          </button>
          <p class="text">Great</p>
        </div>
        <div class="col-4">
          <button type="button" @click="rating('good')">
            <span class="emoji"> &#128578;</span>
          </button>
          <p class="text">Good</p>
        </div>
      </div>
      <div class="row justify-content-center" id="rating-div2">
        <div class="col-4">
          <button type="button" @click="rating('okay')">
            <span class="emoji"> &#128528;</span>
          </button>
          <p class="text">Okay</p>
        </div>
        <div class="col-4">
          <button type="button" @click="rating('bad')">
            <span class="emoji"> &#128533;</span>
          </button>
          <p class="text">Bad</p>
        </div>
      </div>
      <div class="form-group">
        <label>Thanks!! Anything else you'd like to add?</label>
        <textarea
          class="form-control"
          rows="1"
          id="comment"
          v-model="suggestions"
          required
        ></textarea>
      </div>

      <button type="submit" class="btn btn-dark btn-lg btn-block">
        Submit
      </button>
    </form>
  </div>
</template>
<script >

</script>

<style>
body,
html,
.App,
.vue-tempalte,
.vertical-center {
  width: 100%;
  height: 107%;
}
#rating-div > div > button {
  background-color: #ffffff;
  border: none;
}
#rating-div2 > div > button {
  background-color: #ffffff;
  border: none;
}
</style>
