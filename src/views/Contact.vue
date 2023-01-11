<template>
  <section class="contact" id="contact">
    <h2>Get In Touch With Me</h2>
    <div class="contact-form-container">
      <div class="contact-form">
        <form action="https://formspree.io/f/xvowbjaj" method="POST">
          <div class="form-control">
            <label for="name">Name <i class="fas fa-contact-book"></i></label>
            <input
              type="text"
              class="input-field"
              id="name"
              placeholder="Enter Your Name"
              required
            />
          </div>
          <div class="form-control">
            <label for="email">Email <i class="fas fa-mail-bulk"></i></label>
            <input
              type="email"
              class="input-field"
              id="email"
              placeholder="Enter Your Email"
              required
            />
          </div>
          <div class="form-control">
            <label for="message">Message <i class="fas fa-message"></i></label>
            <textarea
              name="message"
              id="message"
              cols="60"
              rows="10"
              placeholder="Enter Your Message"
              class="input-field"
              required
            ></textarea>
          </div>
          <input type="submit" value="submit" id="submit-btn" class="submit-btn" />
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
:root {
  --font-family: "Roboto", sans-serif;
  --normal-font: 400;
  --bold-font: 700;
  --bolder-font: 900;
  --bg-color: #fcfcfc;
  --primary-color: #4756df;
  --secondary-color: #ff7235;
  --primary-shadow: #8b8eaf;
  --secondary-shadow: #a17a69;
  --bottom-margin: 0.5rem;
  --bottom-margin-2: 1rem;
  --line-height: 1.7rem;
  --transition: 0.3s;
  --main-color: red;
}

.form-control-dark {
  border-color: gray;
}
.form-control-dark:focus {
  border-color: #fff;
  box-shadow: 0 0 0 0.25rem rgba(255, 255, 255, 0.25);
}
.contact h2 {
  text-align: center;
  margin-bottom: 1rem;
}

.contact-form-container {
  max-width: 40.75rem;
  margin: auto;
  padding: 0.938rem;
  border-radius: 5px;
  box-shadow: 0 3px 10px #a17a69;
}

.contact-form-container label {
  line-height: 2.7rem;
  font-weight: 400;
  color: #4756df;
}

.contact-form-container .input-field {
  width: 100%;
  padding-top: 10px;
  padding-bottom: 10px;
  border-radius: 5px;
  border: 2px outset #4756df;
  font-size: 0.875rem;
  outline: none;
}

.input-field::placeholder {
  padding: 0.5rem;
  color: #4756df;
}

.submit-btn {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  background-color: #fff;
  border: 2px solid #4756df;
  font-size: 1rem;
  font-weight: 400;
  transition: 0.3s;
}

.submit-btn:hover {
  background-color: #4756df;
  border: 2px solid #4756df;
  cursor: pointer;
}
</style>
