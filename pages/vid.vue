<template>
  <div >
    <p style="text-align:center;margin:1%;font-size:90px">Videos</p>
    <div>
  <youtube :video-id="videoId" class="mx-auto" style="width: 750px;"></youtube>
   </div>
    <div style="display:flex; width: 750px; " class="mx-auto " >
        <div style="margin:2% 30% 0% 5%;">
            <b-button pill variant="primary">Prev</b-button>
        </div>
        <div style="margin:2% 7% 0% 30%;">
            <b-button pill variant="primary">Next</b-button>
        </div>
    </div>
  </div>
</template>

<script>
  export default {
      data () {
    return {
        text: '',
        videoId: "VuN8qwZoego"
      }
      }
  }
</script>
