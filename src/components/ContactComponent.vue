<template>
  <div id="contacts">
    <div class="container" style="padding: 10%">
      <h2>Contact Me</h2>
      <form action="" method="post" enctype="text/plain">
        <div class="form-group">
          <input
            type="email"
            class="form-control"
            v-model="contact.email"
            placeholder="Enter email"
          />
        </div>
        <div class="form-group">
          <textarea
            class="form-control"
            v-model="contact.message"
            rows="3"
            placeholder="Write message"
          ></textarea>
        </div>
      </form>
      <button
        type="button"
        @click.prevent="submit"
        class="btn btn-primary btn-lg"
      >
        Contact
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      contact: {
        email: "",
        message: "",
      },
    };
  },
  methods: {
    submit() {
      if (this.contact.email != "" && this.contact.message != "") {
        this.contact.email = "";
        this.contact.message = "";
      } else {
        alert("All fields are required");
      }
    },
  },
};
</script>