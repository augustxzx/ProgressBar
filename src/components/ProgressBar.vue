<template>
  <div id="progress--wrapper" :style="wrapStyle">
    <div class="progress" :style="pBarStyle">
       <div class="left" :style="percentStyle"></div> 
     </div>   
  </div>   
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    leftColor : String,
    bgColor : String,
    width : String,
    height : String,
    percent:{
      type:Number,
      default:100 
    }
  },
  data () {
    return {
      wrapStyle : {
        'width' : this.width
      },
      pBarStyle : {
        'width' : this.width,
        'height' : this.height   
      },
      percentStyle : {
        'width' : this.percent+'%',
        'height' : this.hegiht,
        'background' :this.leftColor,
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #progress--wrapper {
    width : 100%;
    height : 20px;
    background-color : #ccc;
  }
  .progress {
    width : 50%;
    height : 100% ;
    cursor : point; 
  }
  .left {
    width : 50%;
    height : 100%;
    position : relative;  
  }
</style>
