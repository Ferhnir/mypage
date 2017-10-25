<template>
  <div>
    <div class="container">
      <div class="row new-row-margin">
        <div class="col-lg-12 text-center">
          <h1>Abilities</h1>
          <h3>“A person who never made a mistake never tried anything new.”<br /> - Albert Einstein</h3>
          <hr />
          <h2 class="text-left">Skills</h2>
        </div>
      </div>
      <div class="row text-left">
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in abilities" v-if="index < (abilities.length / 2)">
              <span class="ability-title">{{item.skill}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in abilities" v-if="index > (abilities.length / 2)">
              <span class="ability-title">{{item.skill}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <br />
          <hr />
          <h2 class="text-left">Languages</h2>
        </div>
      </div>
      <div class="row text-left">
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in languages" v-if="index < (languages.length / 2)">
              <span class="ability-title">{{item.lang}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in languages" v-if="index > (languages.length / 2) - 1">
              <span class="ability-title">{{item.lang}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <br />
          <hr />
          <h2 class="text-left">Tools</h2>
        </div>
      </div>
      <div class="row text-left">
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in tools" v-if="index < (tools.length / 2)">
              <span class="ability-title">{{item.tool}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
        <div class="col-md-6">
          <ul class="abilities-list">
            <li v-for="(item, index) in tools" v-if="index > (tools.length / 2)">
              <span class="ability-title">{{item.tool}}</span>
              <span class="ability-score">
                <span v-for="n in 5" class="glyphicon glyphicon-star" v-bind:class="{ 'filled': n < item.level + 1 }"></span>
              </span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'abilities',
  data () {
    return {
      abilities: [
        {skill: 'HTML 5', level: 5},
        {skill: 'CSS 3', level: 4},
        {skill: 'JSON', level: 4},
        {skill: 'MySql', level: 5},
        {skill: 'XML', level: 3},
        {skill: 'JQuery', level: 4},
        {skill: 'PHP', level: 4},
        {skill: 'JavaScript', level: 4},
        {skill: 'Less', level: 3},
        {skill: 'Sass', level: 3},
        {skill: 'Bootstrap framework', level: 5},
        {skill: 'Foundation framework', level: 4},
        {skill: 'MVC Pattern', level: 4},
        {skill: 'OOP', level: 4},
        {skill: 'UML', level: 4},
        {skill: 'AngularJS', level: 4},
        {skill: 'VueJS', level: 2}
      ],
      languages: [
        {lang: 'Polish (Mother language)', level: 5},
        {lang: 'English (Daily use)', level: 5}
      ],
      tools: [
        {tool: 'Firefox', level: 5},
        {tool: 'Chrome', level: 5},
        {tool: 'IE 6+', level: 4},
        {tool: 'Sublime Text', level: 4},
        {tool: 'Atom', level: 4},
        {tool: 'MS Office', level: 5},
        {tool: 'Notepad++', level: 5},
        {tool: 'Windows', level: 5},
        {tool: 'Linux Ubuntu', level: 3},
        {tool: 'Adobe Photoshop', level: 4},
        {tool: 'Adobe Lightroom', level: 4},
        {tool: 'Dreamweaver 6', level: 4},
        {tool: 'Git', level: 4}
      ]
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

  img {
    max-height: 200px;
    max-width: 200px;
    margin-left: auto;
    margin-right: auto;
  }

  .new-row-margin {
    margin-top: 60px;
  }

  .abilities-list {
    list-style-type: none;
    margin: 0px;
    padding: 0px;
  }

  .abilities-list > li {
    height: 40px;
    line-height: 40px;
    padding: 3px 0px;
  }

  .abilities-list > li .ability-title {
    width: 60%;
    display: inline-block;
    font-size: 18px;
  }

  .abilities-list > li .ability-score {
    float: right;
  }

  .abilities-list > li .ability-score .glyphicon {
    color: #e0e0e0;
    padding-right: 5px;
  }

  .abilities-list > li .ability-score .glyphicon.filled {
    color: #22A39F;
  }



</style>
