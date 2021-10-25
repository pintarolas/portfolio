<template>
  <section id="aboutme" class="section">
    <div class="container-fluid justify-content-center">
      <img alt="Foto logo" class="rounded-circle" src="../assets/foto.jpg" />
      <h1>Software Developer</h1>
      <div class="col-12 col-md-4 mx-auto">
        <p>
          I am a software developer in web applications and in creating logical
          and innovative solutions to complex problems. Troubleshooter is
          looking for an entry-level position and eventually a team of
          like-minded developers.
        </p>
      </div>
      <div class="row mx-auto pt-2">
        <div class="col-4 col-md-4 mx-auto">
          <a href="https://github.com/pintarolas" target="_blank">
            <img src="../assets/github.png" alt="github" />
          </a>
          <a href="https://www.linkedin.com/in/jorgefaria91/" target="_blank">
            <img src="../assets/linkedin.png" alt="linkedin" />
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "about-me",
};
</script>

<style scoped>
.section {
  padding-top: 10%;
  padding-bottom: 10%;
  text-align: center;
}

.rounded-circle {
  width: 220px;
  height: 220px;
  margin-top: 1%;
  margin-bottom: 1%;
  border: 2px solid grey;
}
</style>