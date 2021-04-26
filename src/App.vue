<template>
  <div id="app">
      <div class="top-cover" :class="{'active': !active}" >
          <div class="container">
            <template v-for="(item, item_index) in 10" >
              <div :key="item.index" v-if="item <= 5"
              :class="DelayTopLeft(item_index+1)">
              </div>
              <div :key="item.index" v-else
              :class="DelayTopRight(10-item_index)">
              </div>
            </template>
            <template v-for="(item, item_index) in 10" >
              <div :key="item.index" v-if="item <= 5"
              :class="DelayButtomLeft(item_index+1)">
              </div>
              <div :key="item.index" v-else
              :class="DelayButtomRight(10-item_index)">
              </div>
            </template>
          </div>
      </div>
      <full-page :options="options" ref="fullpage" :class="{'opactiy':!active}">
        <div class="section" >
          <Mainpage :active="active" />
        </div>
        <div class="section" >
          <Twopage :active="active"/>
        </div>
        <div class="section" >
          <Threepage :active="active"/>
        </div>
        <div class="section" >
          <Fourpage :active="active"/>
        </div>
        <div class="section">
          <Fivepage :active="active"/>
        </div>
        <div class="section">
          <Sixpage :active="active"/>
        </div>
        <div class="section">
          <Sevenpage :active="active"/>
        </div>
        <div class="section">
          <Eightpage :active="active"/>
        </div>
        <div class="section">
          <Ninepage :active="active"/>
        </div>   
        <div class="section">
          <Tenpage :active="active"/>
        </div>   
        <div class="section">
          <Elevenpage :active="active"/>
        </div>   
        <div class="section">
          <Twelvepage :active="active"/>
        </div>   
        <div class="section">
          <Thirteenpage :active="active"/>
        </div>       
        <div class="section">
          <Fourteenpage :active="active"/>
        </div>          
      </full-page>
  </div>
</template>

<script>
import './assets/css/app.scss';
import Mainpage from './components/mainpage/index';
import Twopage from './components/twopage/index';
import Threepage from './components/threepage/index';
import Fourpage from './components/fourpage/index';
import Fivepage from './components/fivepage/index';
import Sixpage from './components/sixpage/index';
import Sevenpage from './components/sevenpage/index';
import Eightpage from './components/eightpage/index';
import Ninepage from './components/ninepage/index';
import Tenpage from './components/tenpage/index';
import Elevenpage from './components/elevenpage/index';
import Twelvepage from './components/twelvepage/index';
import Thirteenpage from './components/thirteenpage/index';
import Fourteenpage from './components/fourteenpage/index';

export default {
  components: {
    Twopage,
    Mainpage,
    Threepage,
    Fourpage,
    Fivepage,
    Sixpage,
    Sevenpage,
    Eightpage,
    Ninepage,
    Tenpage,
    Elevenpage,
    Twelvepage,
    Thirteenpage,
    Fourteenpage,
  },
  
  name: 'App',
  data() {
    return{
      //fullpage.js
      move:0,
      active:false,
      options: {
        licenseKey: "OPEN-SOURCE-GPLV3-LICENSE",
        //是否顯示導航，預設為false
        navigation: true,
        
        //頁面滾動速度
        scrollingSpeed: 1400,
        //動畫
        controlArrows: true,
        loopBottom:true,
        loopTop:true ,
        onLeave: this.movePage,
        afterLoad: this.movePageAfter,
      },
      //其他
    }
  },

  created () {
    this.timer = setInterval(this.mainBannerMove, 1000)
  },

  methods:{
    mainBannerMove() {
      this.mainpage =! this.mainpage
    },
    movePage(){
      this.active =! this.active
    },
    movePageAfter() {
      this.active =! this.active
    },
    DelayTopLeft(index){
      console.log(index)
        if(!this.active){
            return `animate__animated animate__fadeInTopLeft animate__delay-00`+index+`s`
        }
        else{
            return `animate__animated animate__fadeOutTopLeft animate__delay-00`+index+`s`
        }
    },
    DelayTopRight(index){
      console.log(index)
        if(!this.active){
            return `animate__animated animate__fadeInTopRight animate__delay-00`+index+`s`
        }
        else{
            return `animate__animated animate__fadeOutTopRight animate__delay-00`+index+`s`
        }
    },
    DelayButtomLeft(index){
      console.log(index)
        if(!this.active){
            return `animate__animated animate__fadeInBottomLeft animate__delay-00`+index+`s`
        }
        else{
            return `animate__animated animate__fadeOutBottomLeft animate__delay-00`+index+`s`
        }
    },
    DelayButtomRight(index){
      console.log(index)
        if(!this.active){
            return `animate__animated animate__fadeInBottomRight animate__delay-00`+index+`s`
        }
        else{
            return `animate__animated animate__fadeOutBottomRight animate__delay-00`+index+`s`
        }
    },
  },
  watch:{
    move: function() {
      this.$refs.fullpage.api.moveTo(this.move+1)
    }  
  },
}
</script>
