<template></template>
<script>
export default {
  name: 'scrollSpy',
  props: ['number'],
  data () {
    return {
      myElement: 0
    }
  },
  methods: {
    findWhere () {
    },
    getHeaderPos () {
      this.myElement = document.getElementById('profile').offsetTop
    }
  },
  created () {
    window.addEventListener('scroll', this.findWhere)
    window.addEventListener('load', this.getHeaderPos)
  },
  destroyed () {
    window.removeEventListener('scroll', this.findWhere)
    window.removeEventListener('load', this.getHeaderPos)
  }
}
</script>
