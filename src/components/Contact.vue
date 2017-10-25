<template>
  <div>
    <div class="container">
      <div class="row new-row-margin">
        <div class="col-md-12">
          <h1>Contact</h1>
          <hr />
          <div class="form-field">
            <span class="form-addon">
              <i class="fa fa-user fa-2x"></i>
            </span>
            <input class="form-input-field" type="text" placeholder="Full Name" required>
          </div>
          <div class="form-field">
            <span class="form-addon">
              <i class="fa fa-envelope fa-2x"></i>
            </span>
            <input class="form-input-field" type="text" placeholder="Email" required>
          </div>
          <div class="form-field">
            <span class="form-addon">
              <i class="fa fa-phone fa-2x"></i>
            </span>
            <input class="form-input-field" type="text" placeholder="Phone" required>
          </div>
          <div class="form-field">
            <span class="form-addon">
              <i class="fa fa-info fa-2x"></i>
            </span>
            <input class="form-input-field" type="text" placeholder="Subject" required>
          </div>
          <div class="form-field">
            <span class="form-addon">
              <i class="fa fa-comment fa-2x"></i>
            </span>
            <textarea class="form-input-field" type="text" placeholder="Message" required rows="8"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'contact'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  @import url('https://fonts.googleapis.com/css?family=Josefin+Slab|Noto+Serif|Varela+Round');

  h1, h2, h3, h4 {
    color: rgb(255, 255, 255);
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

  hr {
    border: 0px;
    border-top: 1px solid #6e6e6e;
  }

  .form-field {
    width:100%;
    display: block;
    margin-bottom: 20px;
  }

  .form-addon {
    padding: 8px 20px 8px 20px;
    background-color: #FFF;
    float: left;
    min-width: 80px;
  }

  .form-input-field {
    width: 100%;
    border: 0px;
    display: block;
    line-height: 20px;
    padding: 15px;
    font-size: 16px;
    color: grey;
  }

</style>
