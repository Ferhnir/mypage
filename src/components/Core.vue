<template>
  <div id="PageCoreElement">
    <menu-bar :menu-elements='menuElements' :page-height='pageHeight' ignore></menu-bar>
    <intro-label id="intro" class="full-window centered" ignore></intro-label>
    <profile id="profile" class="bg-white"></profile>
    <experience id="experience" class="bg-grey"></experience>
    <abilities id="abilities" class="bg-white"></abilities>
    <projects id="projects" class="bg-grey"></projects>
    <contact id="contact" class="bg-dark-grey"></contact>
    <scroll-spy ignore></scroll-spy>
  </div>
</template>

<script>
import menuBar from './Menu.vue'
import IntroLabel from './IntroLabel.vue'
import Profile from './Profile.vue'
import Experience from './Experience.vue'
import Abilities from './Abilities.vue'
import Projects from './Projects.vue'
import Contact from './Contact.vue'
import scrollSpy from './scrollspy.vue'

export default {
  name: 'Core',
  components: {
    IntroLabel,
    Profile,
    Experience,
    Abilities,
    Projects,
    Contact,
    menuBar,
    scrollSpy
  },
  data () {
    return {
      number: '999',
      pageHeight: 0,
      menuElements: []
    }
  },
  mounted () {
    var rdElements = this.$children
    for (var i = 0; i < rdElements.length; i++) {
      if (rdElements[i].$el.hasAttribute('id') && !rdElements[i].$el.hasAttribute('ignore')) {
        this.menuElements.push(rdElements[i].$el.getAttribute('id'))
      }
    }
    this.pageHeight = document.getElementById('PageCoreElement').offsetHeight - document.getElementById('intro').offsetHeight
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

  .number {
    position: fixed;
    top: 0px;
    left: 0px;
    width: 100px;
    height: 50px;
    line-height: 50px;
    background-color: white;
    display: block;
    z-index: 10000;
    color: #000;
  }

  .full-window {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    background-color: rgba(14, 14, 14, 0.4);
    }

  .centered {
    display: -webkit-flex;
    display: flex;
    -webkit-align-items: center;
    align-items: center;
  }

  .bg-grey {
    background-color: rgba(252, 248, 248, 1);
  }

  .bg-white {
    background-color: rgba(255, 255, 255, 1);
  }

  .bg-dark-grey {
    background-color: #474747;
  }
</style>
