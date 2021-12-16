<template>
  <form
    class="contact-pg"
    id="fs-frm"
    name="simple-contact-form"
    accept-charset="utf-8"
    action="https://formspree.io/f/xlezelpa"
    method="post"
  >
      <label for="full-name">Full Name</label>
      <input
        type="text"
        name="name"
        id="full-name"
        placeholder="First and Last"
        required=""
      />

      <label for="email-address">Email Address</label>
      <input
        type="email"
        name="_replyto"
        id="email-address"
        placeholder="email@domain.tld"
        required=""
      />

      <label for="message">Message</label>
      <textarea rows="5" name="message" id="message" required="" placeholder="Message here..."></textarea>
      <input
        type="hidden"
        name="_subject"
        id="email-subject"
        value="Contact Form Submission"
      />
    <input type="submit" value="Submit" />
  </form>
</template>

<!-- JS -->
<script>
export default {};
</script>

<!-- CSS -->
<style lang="scss">

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
}

  .contact-pg {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 1rem;
  
  input {
    border: 1px solid gray;
    height: 3rem;
    width: 25rem;
    text-align: center;
    border-radius: 15px;
    margin: 10px;
  }

  textarea {
    width: 25rem;
    border: 1px solid gray;
    border-radius: 5px;
  }

  input[type="submit"] {
    width: max-content;
    background-color: indigo;
    color: white;
    padding: 5px 10px;
    margin: 8px 0;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  input[type="submit"]:hover {
    background-color: #45a049;
  }
}

</style>