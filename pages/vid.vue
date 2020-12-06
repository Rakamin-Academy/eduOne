<template>
  <div >
    <p style="text-align:center;margin:1%;font-size:90px">Videos</p>
    <div class="video-player">
    <div class="video-container">
      <iframe width="640" height="360" :src="this.activeVideo.youtubeURL" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
      <h3 style="text-align:center">{{this.activeVideo.title}}</h3>
      <h4>by {{this.activeVideo.tutor}}</h4>
</div>
    <div class="video-list">
      <p style="font-size:250%;text-align:center">You may Like</p>
    <div style="margin:5%" @click="chooseVideo(video)" :key="video.id" v-for="video in videos" class="thumbnail">
        <div class="thumbnail-img">
          <img :src="video.thumbnail" />
        </div>
        <div class="thumbnail-info">
          <h3>{{video.title}}</h3>
          <p>by {{video.tutor}}</p>
        </div>
    </div>
</div>
  </div>
  </div>
</template>

<script>
let videos=[{
    id: 1,
    title: "Cara mudah pembagian bersusun",
    thumbnail:
      "https://i.ytimg.com/vi/xg7lYD3q0eg/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLAvJvk4k_UNB9nst4pFP-txM1TLZA",
    youtubeURL: "https://www.youtube.com/embed/xg7lYD3q0eg",
    tutor: "Matematika hebat"
  },
  {
    id: 2,
    title: "BELAJAR BERHITUNG PEMBAGIAN 5! TRIK JARIMATIKA CEPAT DAN MUDAH",
    thumbnail:
      "https://i.ytimg.com/vi/tb7DT4Vwwvk/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLDhlan32jHSvicGZezDFPjAOdXGUA",
    youtubeURL: "https://www.youtube.com/embed/tb7DT4Vwwvk",
    tutor: "MA Kids Fun House"
  },
  {
    id: 3,
    title: "Trick Pembagian Semua Angka, Cepat dan Mudah",
    thumbnail:
      "https://i.ytimg.com/vi/95LpfRFAwBw/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLBDnlrC2rVwXamNkicEEbc3Mf4T0w",
    youtubeURL: "https://www.youtube.com/embed/95LpfRFAwBw",
    tutor: "Matematika Spekta"
  },
  {
    id: 4,
    title: "Trik Perkalian Cepat-matematika hebat",
    thumbnail:
      "https://i.ytimg.com/vi/Wpdi1zPwmb0/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLA5hTiwkz4Tr1w1hSMhPlwtmQeyYw",
    youtubeURL: "https://www.youtube.com/embed/Wpdi1zPwmb0",
    tutor: "Matematika Hebat"
  },
  {
    id: 5,
    title: "Cara Menghitung Perkalian Cepat 7 Detik Serba Bisa",
    thumbnail:
      "https://i.ytimg.com/vi/HDXUElGpL40/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLCCxXm7aoPShOwON74nhMlGYMUkHw",
    youtubeURL: "https://www.youtube.com/embed/HDXUElGpL40",
    tutor: "Paman Apiq"
  }];
  export default {
      data () {
    return {
        videoId: "VuN8qwZoego",
        videos,
        activeVideo: videos[1]
      }
      },
      methods:{
  chooseVideo(video){
      //SET VIDEO AS ACTIVE VIDEO
      this.activeVideo = video;
      //INCREASE THE VIDEOS VIEWS BY 1
      video.views += 1;
  },addLike(){
  this.activeVideo.likes += 1;
}
}
  }
</script>

<style>
.thumbnail{
    display:flex;
  }
  .thumbnail img{
    width:168px;
}

.thumbnail-info{
    margin-left:20px;
}

.thumbnail h3{
    font-size:16px;
}

h3,
p{
    margin:0;
    padding:0;
}

.thumbnail-views{
    font-size:14px;
}
.video-player{
    display:flex;
    width:1200px;
    margin:auto;
}

.video-container{
    margin-right:40px;
}

.row{
    display:flex;
    justify-content:space-between;
}

button{
    background:#D0021B;
    color:white;
    border:none;
    padding:10px 20px;
}
</style>