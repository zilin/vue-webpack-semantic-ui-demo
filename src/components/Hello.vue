<template lang="pug">

#hello
  h4.ui.center.aligned.header {{ title }}
  .ui.container.text
    .ui.segments(v-for="video in videos")
      .ui.segment
        .ui.embed(v-bind:data-source="video.source" v-bind:data-id="video.id" v-bind:data-placeholder="video.placeholder")

</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      title: 'Semantic UI Embed Video Demo',
      videos: [
        {'source': 'youtube', 'id': 'O6Xo21L0ybE', 'placeholder': '//semantic-ui.com/images/image-16by9.png'},
        {'source': 'vimeo', 'id': '125292332', 'placeholder': '//semantic-ui.com/images/vimeo-example.jpg'}
      ]
    }
  },
  mounted: function () {
    $('.ui.embed').embed()
  }
}
</script>

<style>
</style>
