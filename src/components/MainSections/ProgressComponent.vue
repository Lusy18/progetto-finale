<template>

  <section class="section_progress" id="progress">
    <div class="area">
      <div class="container">
        <div class="wrapper">
          <div class="left">
            <div class="title"  data-align="left">
              <span>Design is Life</span>
              <h3>I Develop Skills Regularly to Keep Me Update</h3>
              <p>Most common methods for designing websites that work well on desktop is responsive
                and adaptive design</p>
            </div>
            <div class="line_progress" >
              <div class="progress_inner" :style="fastProgressStyle" style="font-weight: bold; " >
                <span>
                  <span class="label" style="width: 85%;  ">Illustrator</span>
                  <span class="number">{{ progress1 }}%</span></span>
                <div class="background">
                  <div class="bar">
                    <div id="orange" class="progress " :class="progressClass1" :style="{ width: progress1 + '%' }" ></div>
                    <div class="bar_in"></div>
                  </div>
                </div>
              </div>
              <div class="progress_inner" style="font-weight: bold;  " >
                <span>
                  <span class="label " style="width: 95%;">Photoshop</span>
                  <span class="number">{{ progress2 }}%</span>
                </span>
                <div class="background">
                  <div class="bar" >
                    <div id="green" class="progress" :class="progressClass2" :style="{ width: progress2 + '%' }" ></div>
                    <div class="bar_in"></div>
                  </div>
                </div>
              </div>
              <div class="progress_inner" style="font-weight: bold;" >
                <span><span class="label " style="width: 75%; ">Figma</span>
                <span class="number">{{ progress3 }}%</span></span>
                <div class="background">
                  <div class="bar">
                    <div  id="purple" class="progress" :class="progressClass3" :style="{ width: progress3 + '%' }" ></div>
                    <div class="bar_in"></div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="right">
            <img src="https://marketifythemes.net/html/dizme/img/skills/2.jpg" alt />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>




<script>


export default {
  name: "ProgressComponent",

  data() {

return {
      progress1: 0,
      progress2: 0,
      progress3: 0,
    };
 },
 computed: {
    progressClass1() {
      return this.progress1 < 85 ? 'orange' : this.progress1 < 85 ? 'green' : 'purple';
    },
    progressClass2() {
      return this.progress2 < 95 ? 'green' : this.progress2 < 95 ? 'green' : 'purple';
    },
    progressClass3() {
      return this.progress3 < 75 ? 'purple' : this.progress3 < 75 ? 'green' : 'purple';
    },
 },
 mounted() {
    this.animateProgress();
 },
 methods: {
    animateProgress() {
      const interval1 = setInterval(() => {
        if (this.progress1 < 85) {
          this.progress1++;
        } else {
          clearInterval(interval1);
        }
      }, 10);

      const interval2 = setInterval(() => {
        if (this.progress2 < 95) {
          this.progress2++;
        } else {
          clearInterval(interval2);
        }
      }, 10);

      const interval3 = setInterval(() => {
        if (this.progress3 < 75) {
          this.progress3++;
        } else {
          clearInterval(interval3);
        }
      }, 10);
    },
  }
}
    
  










</script>





<style scoped>

.title {
  width: 100%;
  max-width: 680px;
  height: auto;
  clear: both;
  text-align: left;
  margin: 0 auto
}

.title h3 {
  font-size: 40px;
  line-height: 1.25;
  margin-bottom: 23px
}

.title p{
    color:#9e9cad;
    font-size: 18px;
}


.title span {
  font-size: 24px;
  font-weight: 500;
  color: #f75023;
  font-family: 'jost', sans-serif;
  display: inline-block;
  margin-bottom: 6px;
}

.area .right {
  width: 50%;
  padding-left: 100px;
  padding-top:150px;
}

.area .right img {
  max-height: 650px
}


.area {
  width: 100%;
  height: auto;
  display: left
}

.area .wrapper {
  width: 100%;
  height: auto;
  clear: both;
  display: flex;
  align-items: center
}

.area .left {
  width: 50%;
  padding-right: 100px
}

.line_progress {
  width: 100%;
  height: auto;
  clear: both;
  display: left;
  padding-top: 30px;
  overflow: hidden;
  
}

.line_progress .progress_inner:last-child {
  margin-bottom: 0
  
}


.progress_inner {
  width: 100%;
  margin-bottom: 22px;
 

}


.progress_inner span {
  margin: 0 0 9px;
  display: flex;
  text-align: left;
  position: relative;
  

} 



.progress_inner .background {
  background: white;
  width: 100%;
  min-width: 100%;
  position: relative;
  height: 8px;
  border-radius: 50px;
  
}


.progress {
  border-radius: 50px;
  height: 8px;
}


#green{
  background-color: green;

}

#orange {

background-color: #f75023;

}

#purple{
  background-color: #9e4caf;
}

.number{
  color: orangered;
  

} 





</style>