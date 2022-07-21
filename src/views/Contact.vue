<template>
  <div class="contact">
    <h1>Find Me</h1>
      <form action="https://formspree.io/f/xvolzybv" method="POST">
         <div class="container py-5">
               <h3>Contact Form</h3>
      <div class="row">
        <col-12 class="mb-3">
          <input
            class="form-control"
            placeholder="Email"
            type="email"
            name="_replyto"
          />
        </col-12>
        <col-12 class="mb-3">
          <textarea
            class="form-control"
            placeholder="Message"
            name="message"
          ></textarea>
        </col-12>
      </div>
      <button class="btn btn-primary " type="submit">Send</button>
    </div>
  </form>
  

  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.contact {
   
    height: 90vh;
   
}

</style>