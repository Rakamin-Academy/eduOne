<template>
    <b-container class="" style="margin-top:5%;">
  <b-row align-v="start">
    <b-col style="text-align:left;">
      <h3 style="margin-bottom:5%;">Lorem ipsum dolor sit amet consectetur adipisicing.</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ullam deleniti, facilis fugit harum consequuntur perspiciatis a alias dicta repudiandae nostrum odit amet suscipit.</p>
        <nuxt-link to="/Videos">Learn More >></nuxt-link>
    </b-col>
    <b-col>
    <div>
  <youtube :video-id="videoId"></youtube>
   </div>
    </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
    name: 'Video',
    data () {
    return {
        text: '',
        videoId: "VuN8qwZoego"
      }
  }
}
</script>

<style>

</style>