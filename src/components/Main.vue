<template>
  <b-container class="bv-example-row main">
    <b-row>
      <b-col cols="8">
        <div id="vue-core-video-player-box" class="example-player">
          <vue-core-video-player  :src="currentMovie.source"></vue-core-video-player>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
// import DATA from '../assets/data'

// let movie = DATA[2]

// const videoSource = [
//   {
//     src: 'https://media.vued.vanthink.cn/sparkle_your_name_am360p.mp4',
//     resolution: 360,
//   }, {
//     src: 'https://media.vued.vanthink.cn/sparkle_your_name_am720p.mp4',
//     resolution: 720,
//   }, {
//     src: 'https://media.vued.vanthink.cn/y2mate.com%20-%20sparkle_your_name_amv_K_7To_y9IAM_1080p.mp4',
//     resolution: 1080
//   }
// ]
// const DATA = [
// {
//   source:videoSource[0].src ,
// }, 
  
// {
//   source: videoSource[2].src,
// },  
// {
//   source: videoSource,
// }, 
// ];
export default {
  name: 'Main',
  components: {
  },
  data() {
    return {
      currentMovie: null,
      // currentMovie: DATA[2],
    }
  },
  created(){
      const videoSource = [
        {
          src: 'https://media.vued.vanthink.cn/sparkle_your_name_am360p.mp4',
          resolution: 360,
        }, {
          src: 'https://media.vued.vanthink.cn/sparkle_your_name_am720p.mp4',
          resolution: 720,
        }, {
          src: 'https://media.vued.vanthink.cn/y2mate.com%20-%20sparkle_your_name_amv_K_7To_y9IAM_1080p.mp4',
          resolution: 1080
        }
      ]
    const DATA = [
      {
        source:videoSource[0].src ,
      }, 
      {
        source: videoSource[2].src,
      },  
      {
        source: videoSource,
      }, 
    ];
    this.currentMovie = DATA[2]
  },
  methods: {
    // open() {
    //   window.open('https://github.com/core-player/vue-core-video-player-examples')
    // }
  },
}
</script>

<style>
  .example-player {
    position: relative;
    height: 410px;
    background-color: #000;
    font-weight: normal;
  }
  .movie-detail{
    padding-top: 20px;
    color: rgba(0,0,0, .65);
  }
  .movie-detail h1{
    font-size: 20px;
    color: #000;
  }
  .movie-detail .date {
    font-size: 14px;
  }
  .movie-detail .desc {
    font-size: 13px;
    padding: 10px 20px 10px 0;
  }
  .movie-detail .btn-wrap {
    padding-right: 20px;
    text-align: right;
  }
  .play-list h2 {
    font-size: 18px;
    color: rgba(0,0,0, .85);
    padding-bottom: 10px;
  }
  .recommend-list {
    margin-top: 40px;
    padding-top: 40px;
    padding-bottom: 40px;
    border-top: 1px solid #ddd;
  }
  .thanks {
    padding: 20px 0 40px;
    color: rgba(0, 0, 0, .25);
    font-size: 13px;
    text-align: center;
  }
  .recommend-list:after{
    content: '';
    display: block;
    clear: both;
  }
</style>
