<template>
  <div>
    <div class="container">
      <div class="row new-row-margin">
        <div class="col-lg-12 text-center">
          <h1>Projects</h1>
          <h3>"You can do anything you set your mind to."<br /> - Benjamin Franklin</h3>
          <hr />
        </div>
      </div>
      <div class="row new-row-margin">
        <div class="col-md-6">
          <a href="http://dec-sado.co.uk" class="project-links" target="_blank">
            <img src="../assets/dec-sado.png" alt="www.dec-sado.co.uk" class="img-thumbnail img-responsive">
            <h4>
              www.Dec-Sado.co.uk
            </h4>
          </a>
        </div>
        <div class="col-md-6">
          <a href="http://dec-sado.co.uk" class="project-links" target="_blank">
            <img src="../assets/dec-sado.png" alt="www.dec-sado.co.uk" class="img-thumbnail img-responsive">
            <h4>
              www.Dec-Sado.co.uk
            </h4>
          </a>
        </div>
      </div>
      <div class="row new-row-margin"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'projects'
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

  h2, h3, .abilities-list > li .ability-title {
    font-family: 'Josefin Slab', serif;
  }

  h2 {
    font-size: 30px;
  }

  h3 {
    font-size: 20px;
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

  .new-row-margin {
    margin-top: 60px;
  }

  .project-links{
    color: #000;
    cursor: pointer;
  }
</style>
