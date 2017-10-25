<template>
  <div>
    <div class="container">
      <div class="row new-row-margin">
        <div class="col-lg-12 text-center">
          <h1>Experience</h1>
          <h3>"Try not to become a man of success, but rather try to become a man of value."<br /> - Albert Einstein</h3>
          <hr />
          <h2 class="text-left">Educations</h2>
        </div>
      </div>
      <div class="row text-left">
        <div class="col-md-4">
          <B>Higher School of IT - "WISZ"</B>
          <h5>2002 - 2007</h5>
        </div>
        <div class="col-md-8">
          <B>Bachelor - Computer Engineering <br />(Specialization: Microprocessor Systems Steerings)</B>
          <h5>The education was mainly study about electronics and low level programing such as assembler, C and other machine languages, but also learned about C++, PHP, JavaScript and Sql.
            During my time in college, I specialized in Microprocessor systems which allowed me to udnerstand computer technologies.</h5>
        </div>
      </div>
      <div class="row new-row-margin">
        <div class="col-lg-12 text-center">
          <hr />
          <h2 class="text-left">Careers</h2>
        </div>
      </div>
      <div class="row text-left">
        <div class="col-md-4">
          <B>"Webz-Studio"</B>
          <h5>2014 - current</h5>
        </div>
        <div class="col-md-8">
          <B>Buisness owner</B>
          <h5>In 2014 I founded own buisness. Providing service like a creating new websites but also adding or editing scripts on exsting ones.
              My work is mainly focused on small and medium companies.</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'experience',
  data () {
    return {
      msg: 'Welcome stranger!'
    }
  }
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
