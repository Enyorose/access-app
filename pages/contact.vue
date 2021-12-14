<template>
  <main>
    <div>
      <Header />
    </div>
    <!--map-->
    <section>
      <iframe
        width="600"
        height="450"
        style="border: 0"
        loading="lazy"
        allowfullscreen
        src="https://www.google.com/maps/embed/v1/search?q=Bow%20Valley%20Square%2C%205%20Avenue%20Southwest%2C%20Calgary%2C%20AB%2C%20Canada&key=AIzaSyD6ImALDdeRhFlJaeF7P6dN33JmYNCu26c"
      ></iframe>
      <!--form-->
      <form
        id="fs-frm"
        name="simple-contact-form"
        accept-charset="utf-8"
        action="https://formspree.io/f/xlezelpa"
        method="post"
      >
        <fieldset id="fs-frm-inputs">
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
          <textarea rows="5" name="message" id="message" required=""></textarea>
          <input
            type="hidden"
            name="_subject"
            id="email-subject"
            value="Contact Form Submission"
          />
        </fieldset>
        <input type="submit" value="Submit" />
      </form>
    </section>
  </main>
</template>
<script>
export default {
  data() {
    return {
      pageInfo: {
        menuName: "contact",
        header: "Contact",
      },
    };
  },
};
</script>

<style lang="scss">
section {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  text-align: center;
  align-items: center;
  align-content: center;
}
</style>