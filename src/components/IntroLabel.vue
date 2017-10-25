<template>
  <div>
    <div class="container">
      <div class="row">
        <div id="IntroPage" ref="introLabel">
          <div class="col-lg-3"></div>
          <div class="panel col-lg-6">
            <div class="panel-body">
              <h1>Maskymilian Zdunski</h1>
              <hr />
              <h2>Interactive resume</h2>
            </div>
          </div>
          <div class="col-lg-3"></div>
        </div>
      </div>
    </div>
    <div class="trigger-down">
      <span class="glyphicon glyphicon-arrow-down"></span>
    </div>
  </div>
</template>
<script>

export default {
  name: 'introLabel',
  data () {
    return {
      msg: 'Welcome stranger!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  @import url('https://fonts.googleapis.com/css?family=Baloo+Bhaina|Lobster');

  #IntroPage > * {
    color: #FFF;
  }

  h1 {
    font-family: 'Baloo Bhaina', cursive;
    font-size: 20px;
  }

  h2 {
    font-family: 'Lobster', cursive;
    font-size: 15px;
  }

    @media (min-width: 768px) {
      h1 {
        font-size: 40px;
      }

      h2 {
        font-size: 25px;
      }
    }

  .panel {
    background-color: rgba(63, 191, 127, 0.6);
  }

  .panel-default {
    border-color: rgba(0,0,0,0.1);
  }

  .trigger-down {
      position: absolute;
      bottom: 0px;
      right: 5%;
      background-color: rgb(63, 191, 127);
      width: 120px;
      border: none;
      border-radius: 7px 7px 0px 0px;
      display: block;
      height: 90px;
      line-height: 90px;
      color: #FFF;
      font-size: 30px;
      padding: 8px 0px;
  }

  .margin-both-10 {
    margin-left: 10px;
    margin-right: 10px;
  }
</style>
