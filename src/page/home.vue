<template>
  <div class="hd-home">
      <div class="home-first" :class="{hide:hide}">
      <div class="home-header">
          <div class="header-h1">
              <span class="h1-en">BGI·MARINE</span><br>
              <span  class="h1-zh">华大海洋</span>
          </div>
          <div class="header-fun">
             <span class="home-search-input">
                 <input type="text"/>
                 <span class="iconfont icon-sou"></span>
             </span>
             <span class="fun-lang">
                  <span>简 </span>
                    <span> | </span>
                    <span> EN</span>
             </span>
            
          </div>
      </div>
      <div class="home-nav">
          <ul class="hd-nav-ul">
            <li>首页</li>
            <li>关于我们</li>
            <li>核心优势领域</li>
            <li>业务模块</li>
            <li>水产品研发及精准营养</li>
            <li>大数据</li>
          </ul>
      </div>
      <div class="center-h1">
          <span>
              大数据
          </span>
          <br>
          <span class="center-en">
              Big data
          </span>

      </div>
      <div class="page-down" @click="hide=true">
          <span class="iconfont icon-down-trangle " :class="{light:num%3==0}"></span><br>
           <span class="iconfont icon-down-trangle"  :class="{light:num%3==1}"></span><br>
            <span class="iconfont icon-down-trangle"  :class="{light:num%3==2}"></span>
      </div>
      </div>
      <div class="home-sec" :class="{show:hide}">
          <div class="hd-center">
              <div class="hd-center-bg" v-show="showBg">

              </div>
              <div class="hd-center-ball" v-show="showBall">
                                     <div>打发我的<br>打发我的</div> 
              </div>
              <div class="hd-center-ball-l" v-show="showBalls">
                    <div>打发我的<br>打发我的</div>
              </div>
               <div class="hd-center-ball-r" v-show="showBalls">
                    <div>打发我的</div>
              </div>
              <div class="hd-tra hd-tra-1" v-show="showTrg">

              </div>
               <div class="hd-tra hd-tra-2"  v-show="showTrg">

              </div>
               <div class="hd-tra hd-tra-3"  v-show="showTrg">

              </div>
               <div class="hd-tra hd-tra-4"  v-show="showTrg">

              </div>
               <div class="hd-tra hd-tra-5"  v-show="showTrg">

              </div>
                <div class="hd-tra hd-tra-6"  v-show="showTrg">

              </div>

                <div class="hd-c-text hd-c-text-1"  v-show="showText">
                    <span>打发我的伟大</span>
              </div>
                              <div class="hd-c-text hd-c-text-2"  v-show="showText">
                    <span>打发我的伟大</span>
              </div>
                              <div class="hd-c-text hd-c-text-3"  v-show="showText">
                    <span>打发我的伟大</span>
              </div>
                  <div class="hd-c-text hd-c-text-4"  v-show="showText">
                    <span>打发我的伟大</span>
              </div>
                              <div class="hd-c-text hd-c-text-5"  v-show="showText">
                    <span>打发我的伟大</span>
              </div>

             <div class="hd-c-text hd-c-text-l1"  v-show="showText">
                    <span>打发我的伟</span>
              </div>
               <div class="hd-c-text hd-c-text-l2"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-l3"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-l4"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-l5"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-l6"  v-show="showText">
                    <span>打发我的</span>
              </div>
              <div class="hd-c-text hd-c-text-r1"  v-show="showText">
                    <span>打发我的</span>
              </div>
                           <div class="hd-c-text hd-c-text-r2"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-r3"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-r4"  v-show="showText">
                    <span>打发我的</span>
              </div>
               <div class="hd-c-text hd-c-text-r5"  v-show="showText">
                    <span>打发我的</span>
              </div>
               
          </div>
          
      </div>
  </div>
</template>
<script>
    export default {
        data(){
            return {
                num:0,
                hide:true,
                showBg:false,
                showTrg:false,
                showText:false,
                showBall:false,
                showBalls:false
            };
        },
        mounted () {
            setInterval(()=>{
                this.num++
            },500)
            this.setAnimation()
        },
        methods : {
            setAnimation(){
                setTimeout(()=>{
                    this.showBg = true
                },1500)
                setTimeout(()=>{
                    this.showBall = true
                },1)  
                setTimeout(()=>{
                    this.showTrg = true
                },1000)  
                 setTimeout(()=>{
                    this.showBalls = true
                },1000)  
            }
        }
    }
</script>
<style lang="scss">
.hd-home{
    height: 100%;
    box-sizing: border-box;
    overflow: hidden;
}
.home-first{
    height: 100%;
    padding-top: 60px;
    background: url("https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1515519801721&di=4a01e793243ed115cd4b5cb8bd453e3c&imgtype=0&src=http%3A%2F%2Fimg.zcool.cn%2Fcommunity%2F0144ca5943cf88a8012193a3ce0d5f.jpg") no-repeat;
    background-size: 100% auto;
    position: relative;
    top: 0;
    transition: top .5s;
    &.hide{
        top: -100%;
        transition: top .5s;
    }
    box-sizing: border-box;
    height: 100%;
    overflow: hidden;
}

.home-header{
    color: #fff;
    position: relative;
    width: 1200px;
    margin: 0px auto 0;
}
.header-h1{
    display: inline-block;
    margin-left: 550px;
    .h1-en{
        font-size: 18px;
    }
    .h1-zh{
        font-size: 14px;
    }

}
.header-fun{
    position: absolute;
    right: 0;
    bottom: 0;
    color: #004a64;
}
.home-nav{
    width: 1200px;
    margin: 60px auto;
}
.hd-nav-ul{
    background: #004a64;
    color: #fff;
    overflow: hidden;
    padding-left: 190px;
    li {
        list-style: none;
        float: left;
        margin-right: 50px;
        padding:28px 0 23px;
        border-bottom: 5px solid #004a64;
    }
    li:hover{
         border-bottom: 5px solid #f1dd24;
         cursor: pointer;
    }
}
.center-h1{
    margin-top: calc(50vh - (240px));
    font-size: 50px;
    color: #fff;
    text-align: center;
}
.center-en{
    font-size: 36px;
}
.fun-lang{
    font-size: 14px;
    span{
        margin: 0 3px;
        cursor: pointer;
    }
}
.home-search-input{
    position: relative;
    display: inline-block;
    vertical-align: middle;
    margin:0 10px;
    input {
        height: 30px;
        width: 100px;
        border-radius: 15px;
        border: none;
        outline: none;
        padding:0 30px;
        background: rgba(255, 255, 255, .3);
        color:#fff;
    }
    span{
        position: absolute;
        font-size: 20px;
        right: 10px;
        top: 2px;
        color:#004a64;
        cursor: pointer;
    }
}
.page-down{
    position: absolute;
    bottom: 70px;
    width: 100%;
    text-align: center;
    color: #aaa;
    line-height: 8px;
    .iconfont{
        font-size: 24px;
        &.light{
            color: #fff;
        }
    }
    
}
.home-sec{
    height: 100%;
    background: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    top: 0;
    transition: top .5s;
    &.show{
        top: -100%;
        transition: top .5s;
    }
}
.hd-center{
    width: 600px;
    height: 600px;
    position: relative;
}
.hd-center-bg{
    position: absolute;
    height: 100%;
    width: 100%;
    background: url(../assets/ctbg.png);
    background-size: 100% 100%;
    animation: rotate 1.5s ease-out;
}
.hd-center-ball{
    width: 150px;
    height: 150px;
    background:url(../assets/bg.png);
    background-size: 100% 100%;
    border-radius: 50%;
    position: absolute;
    top: 225px;
    left: 225px;
     display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #fff;
    animation: scale .5s linear;
}
.hd-center-ball-l{
    font-size: 12px;
    width: 80px;
    height: 80px;
     background:url(../assets/bg.png);
    background-size: 100% 100%;
    border-radius: 50%;
    position: absolute;
    top: 260px;
    left: 95px;
    text-align: center;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    animation: scale .5s linear;
}
.hd-center-ball-r{
    font-size: 12px;
    width: 80px;
    height: 80px;
     background:url(../assets/bg.png);
    background-size: 100% 100%;
    border-radius: 50%;
    position: absolute;
    color: #fff;
    top: 260px;
    left: 425px;
     display: flex;
     text-align: center;
    align-items: center;
    justify-content: center;
    animation: scale .5s linear;
}
.hd-tra{
    position: absolute;
    height: 0;
    width: 0;
    border-top: #f5e023 12px solid;
    border-bottom: transparent 12px solid;
    border-left: transparent 12px solid;
    border-right: transparent 12px solid;
    animation: opacity 1s linear;
  
}
.hd-tra-1{
    top: 150px;
    left: 288px;
    transform: rotate(180deg)
}
.hd-tra-2{
    top: 190px;
    left: 288px;
}
.hd-tra-3{
    top: 288px;
    left: 194px;
    transform: rotate(-90deg)
}
.hd-tra-4{
    top: 288px;
    left: 394px;
    transform: rotate(-90deg)
}
.hd-tra-5{
    top: 380px;
    left: 288px;
    transform: rotate(-180deg)
}
.hd-tra-6{
    top: 500px;
    left: 288px;
    transform: rotate(-180deg)
}
.hd-c-text{
    position: absolute;
    background: #fff;
    border-radius: 15px;
    border: 3px solid #004962;
    padding:15px 30px;
    font-size: 20px;
    transform: scale(.5,.5);
    word-break: keep-all;
    white-space: nowrap;
    color: #004a64;
    animation: slidown .5s linear;
}
.hd-c-text-1{
    top: 20px;
    left: 140px;
}
.hd-c-text-2{
    top: 20px;
    left: 270px;
}
.hd-c-text-3{
    top: 60px;
    left: 205px;
}
.hd-c-text-4{
    top: 430px;
    left: 205px;
}
.hd-c-text-5{
    top: 530px;
    left: 205px;
}
.hd-c-text-l1{
    top: 105px;
    left: 35px;
}
.hd-c-text-l2{
    top: 170px;
    left: 5px;
}
.hd-c-text-l3{
    top: 235px;
    left: -20px;
}
.hd-c-text-l4{
    top: 300px;
    left: -20px;
}
.hd-c-text-l5{
    top: 365px;
    left: 5px;
}
.hd-c-text-l6{
    top: 430px;
    left: 35px;
}
.hd-c-text-r1{
    top: 110px;
    left: 400px;
}
.hd-c-text-r2{
    top: 190px;
    left: 440px;
}
.hd-c-text-r3{
    top: 270px;
    left: 480px;
}
.hd-c-text-r4{
    top: 350px;
    left: 440px;
}
.hd-c-text-r5{
    top: 430px;
    left: 400px;
}
</style>
<style lang="scss">
			@keyframes scale
			{
				from {transform: scale(.1,.1);}
				to {transform: scale(1,1);}
			}
			@keyframes slidown
			{
				from {height: 0;}
				to {height:30px;}
			}
			@keyframes opacity
			{
				from {opacity: 0;}
				to {opacity:1}
			}
            @keyframes rotate
			{
				from {transform: rotate(0deg);opacity: 0;}
				to {transform: rotate(720deg);opacity:1}
			}
</style>

