<template>
  <div>
    <div id="menu-bar" v-bind:class="sticky">
      <div id="pointer2">
        <div class="left-triag">
          <div class="left-triag-shape"></div>
        </div>
        <div class="center-bar">
          <div class="top-pointer"></div>
          <div class="bottom-pointer"></div>
        </div>
        <div class="right-triag">
          <div class="right-triag-shape"></div>
        </div>
      </div>
      <ul class="menu-list">
        <li v-for="menu in menuElements">
          <a v-bind:href="menu.href">{{ menu }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'menuBar',
  props: [ 'menuElements', 'pageHeight' ],
  data () {
    return {
      sticky: 'absolute',
      wHeight: 0,
      spyHeight: 0
    }
  },
  methods: {
    handleScroll () {
      if (window.scrollY > this.wHeight && this.sticky !== 'fixed') {
        this.sticky = 'fixed'
        console.log(this.props.pageHeight)
      }
      if (window.scrollY < this.wHeight && this.sticky !== 'absolute') {
        this.sticky = 'absolute'
      }
    },
    handleResize () {
    }
  },
  created () {
    this.wHeight = window.innerHeight
    window.addEventListener('scroll', this.handleScroll)
    window.addEventListener('resize', this.handleResize)
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll)
    window.removeEventListener('resize', this.handleResize)
  },
  mounted () {
  }
}
</script>

<style scoped>
  #pointer {
    position: relative;
    width: 0;
    height: 0;
    border-top: 10px solid transparent;
    border-left: 20px solid red;
    border-bottom: 10px solid transparent;
    top: -10px;
    left: -20px;
  }

  #pointer2 {
    position: absolute;
    width: 160px;
    height: 20px;
    top: 35px;
    left: -20px;
    z-index: 90;
  }

  .left-triag,
  .right-triag {
    float: left;
    width: 20px;
    height: 20px;
    background-color: rgb(63, 191, 127);
  }

  .left-triag {
    border-top-left-radius: 10px;
    border-bottom-left-radius: 10px;
  }

  .right-triag {
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
  }

  .left-triag-shape {
    margin-top: 5px;
    float: right;
    border-top: 5px solid transparent;
    border-left: 10px solid #FFF;
    border-bottom: 5px solid transparent;
  }

  .right-triag-shape {
    margin-top: 5px;
    float: left;
    border-top: 5px solid transparent;
    border-right: 10px solid #FFF;
    border-bottom: 5px solid transparent;
  }

  .center-bar {
    float: left;
  }

  .top-pointer {
    display: block;
    width: 120px;
    height: 10px;
  }

  #menu-bar {
    right: 5%;
    background-color: rgb(63, 191, 127);
    width: 120px;
    border: none;
    border-radius: 0px 0px 7px 7px;
  }

  .absolute {
    position: absolute;
    top: 100%;
    z-index: 100;
  }

  .fixed {
    position: fixed;
    top: 0px;
  }

  .menu-list {
    list-style: none;
    padding: 0px;
    margin: 0px;
  }

  .menu-list > li {
    height: 90px;
    line-height: 90px;
    padding: 0px;
    margin: 0px;
  }

  .menu-list > li > a {
    text-decoration: none;
    font-weight: bold;
    color: #FFF;
    transition: 0.5s;
    display: block;
  }

  .menu-list > li > a:first-letter {
    text-transform: uppercase;
  }

  .menu-list > li > a:hover,
  .menu-list > li > a:active {
    background-color: #000;
    transition: 0.5s;
  }
</style>
