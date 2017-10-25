<template>
  <div>
    <div class="container">
      <div class="row new-row-margin">
        <div class="col-lg-12">
          <h1>Profile</h1>
          <h3>I'm creative webdeveloper</h3>
        </div>
      </div>
      <hr />
      <div class="row new-row-margin">
        <div class="col-md-4 text-left">
          <h2>About Me</h2>
          <h5>I am a self-taught, enthusiastic developer. I consider myself to be an open minded individual, who is keen to learn new things.
            My portfolio to date consists of back-end and front-end techniques, with my latest work primarily focused on front-end.
            I thrive on individual work, as well as working as part of a team</h5>
        </div>
        <div class="col-md-4">
          <img src="../assets/prof_pic.jpg" class="img-circle img-responsive" />
        </div>
        <div class="col-md-4 text-left">
          <h2>Details</h2>
          <h5><b>Name:</b><br />
          Maksymilian Zdunski</h5>
          <h5><b>dob:</b><br />
          15 november 1984</h5>
          <h5><b>Location:</b><br />
          Manchester, Ashton-under-Lyne</h5>
        </div>
      </div>
      <div class="row new-row-margin"></div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'profile'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  @import url('https://fonts.googleapis.com/css?family=Josefin+Slab|Noto+Serif|Varela+Round');

  h1, h2 {
    color: rgb(63, 191, 127);
  }

  h1, h4 {
    font-family: 'Varela Round', sans-serif;
    font-size: 40px;
  }

  h2, h3 {
    font-family: 'Josefin Slab', serif;
  }

  h2 {
    font-size: 30px;
  }

  h3 {
    font-size: 25px;
  }

  h4 {
    font-weight: bold;
    font-size: 17px;
    }

  h5 {
    font-family: 'Noto Serif', serif;
    font-size: 14px;
    line-height: 27px;
  }

  img {
    max-height: 200px;
    max-width: 200px;
    margin-left: auto;
    margin-right: auto;
  }

  .new-row-margin {
    margin-top: 60px;
  }


</style>
