<template>
  <div class="index-wrap">
    <slide-show :slides="slides"></slide-show>
  </div>
</template>

<script>
import slideShow from './components/slideShow'
export default {
  components: {
    slideShow
  },
  data () {
    return {
      slides: [
        {
          src: require('./assets/1.jpg'),
          title: 'xxx1',
        },
        {
          src: require('./assets/2.jpg'),
          title: 'xxx2',
        },
        {
          src: require('./assets/3.jpg'),
          title: 'xxx3',
        },
        {
          src: require('./assets/4.jpg'),
          title: 'xxx4',
        },
        {
          src: require('./assets/5.jpg'),
          title: 'xxx5',
        }
      ]
    }
  }
}
</script>

<style scoped>
  .index-wrap {
    overflow: hidden;
}
</style>
