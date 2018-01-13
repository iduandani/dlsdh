<template>
  <div class="hd-home">
      <div class="home-first" >
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
      <div class="page-down" @click="showMore">
          <span class="iconfont icon-down-trangle " :class="{light:num%3==0}"></span><br>
           <span class="iconfont icon-down-trangle"  :class="{light:num%3==1}"></span><br>
            <span class="iconfont icon-down-trangle"  :class="{light:num%3==2}"></span>
      </div>
      </div>
      <div class="home-sec" v-show="showmore">
          <div class="hd-center">
              <div class="hd-center-bg" v-show="showBg">

              </div>
              <div class="hd-center-ball" v-show="showBall">
                                     <div>水产大数据<br>中心</div> 
              </div>
              <div class="hd-center-ball-l" v-show="showBalls">
                    <div>数据输入<br>与维护</div>
              </div>
               <div class="hd-center-ball-r" v-show="showBalls">
                    <div>增值服务</div>
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

                <div class="hd-c-text hd-c-text-1"  v-show="showText1">
                    <span>数据存储中心</span>
              </div>
                              <div class="hd-c-text hd-c-text-2"  v-show="showText1">
                    <span>样本保存中心</span>
              </div>
                              <div class="hd-c-text hd-c-text-3"  v-show="showText2">
                    <span>活体展示中心</span>
              </div>
                  <div class="hd-c-text hd-c-text-4"  v-show="showText8">
                    <span>计算机硬件</span>
              </div>
                              <div class="hd-c-text hd-c-text-5"  v-show="showText9">
                    <span>运营支持团队</span>
              </div>

             <div class="hd-c-text hd-c-text-l1"  v-show="showText3">
                    <span>生物学数据</span>
              </div>
               <div class="hd-c-text hd-c-text-l2"  v-show="showText4">
                    <span>养殖数据</span>
              </div>
               <div class="hd-c-text hd-c-text-l3"  v-show="showText5">
                    <span>市场数据</span>
              </div>
               <div class="hd-c-text hd-c-text-l4"  v-show="showText6">
                    <span>组学数据</span>
              </div>
               <div class="hd-c-text hd-c-text-l5"  v-show="showText7">
                    <span>种业数据</span>
              </div>
               <div class="hd-c-text hd-c-text-l6"  v-show="showText8">
                    <span>产业数据</span>
              </div>
              <div class="hd-c-text hd-c-text-r1"  v-show="showText3">
                    <span>数据查询</span>
              </div>
                           <div class="hd-c-text hd-c-text-r2"  v-show="showText4">
                    <span>数据分析</span>
              </div>
               <div class="hd-c-text hd-c-text-r3"  v-show="showText5">
                    <span>技术服务</span>
              </div>
               <div class="hd-c-text hd-c-text-r4"  v-show="showText6">
                    <span>市场趋势分析</span>
              </div>
               <div class="hd-c-text hd-c-text-r5"  v-show="showText8">
                    <span>产业发展咨询</span>
              </div>
               
          </div>
          
      </div>
      <div class="center-tips"  v-show="showmore">
          <div class="tip-top">水产生物大数据</div>
          <div><span class="tips-div"></span></div>
          <div  class="tips-c">
              <span>逐步收集并完善水产生物的生物学数据、组学数据、养殖数据、种业数据、市场数据和产业数据，通过水产大数据中心的分析运行，实现
             数据查询、数据分析、技术服务、市场趋势分析和产业发展咨询等增值服务。</span>
          </div>
      </div>
      <div  v-show="showmore">
            <div class="center-btns">
                <span>点击查看数据库</span>
            </div>    
      </div>
      <div class="footer"  v-show="showmore">
          <div class="footer-l">
              <div class="footer-ul">
                  <div class="ul-title">关于我们</div>
                   <ul>
                  
                  <li>
                      <a href="javascript:;">企业简介</a>
                  </li>
                  <li>
                      <a href="javascript:;">企业文化</a>
                  </li>
                  <li>
                      <a href="javascript:;">专业论著</a>
                  </li>
                  <li>
                      <a href="javascript:;">专家介绍</a>
                  </li>
                  <li>
                      <a href="javascript:;">招聘</a>
                  </li>
                  <li>
                      <a href="javascript:;">新闻资讯</a>
                  </li>
              </ul>
              
              </div>
              <div class="footer-ul">
                  <div class="ul-title">核心优势领域</div>
                   <ul>
                  
                  <li>
                      <a href="javascript:;">分子育种</a>
                  </li>
                   <li>
                      <a href="javascript:;">立体循环水生态养殖</a>
                  </li>
                    <li>
                      <a href="javascript:;">深加工</a>
                  </li>
                  
              </ul>
              
              </div>
                            <div class="footer-ul">
                  <div class="ul-title">业务模块</div>
                   <ul>
                  
                  <li>
                      <a href="javascript:;">育种与种业</a>
                  </li>
                   <li>
                      <a href="javascript:;">国内外贸易</a>
                  </li>
              </ul>
              
              </div>
                            <div class="footer-ul">
                  <div class="ul-title">水产品研发及精准营养</div>
                   <ul>
                  
                  <li>
                      <a href="javascript:;">热销商品</a>
                  </li>
                   <li>
                      <a href="javascript:;">鲜活产品</a>
                  </li>
                    <li>
                      <a href="javascript:;">深加工产品</a>
                  </li>
                  
              </ul>
              
              </div>
                            <div class="footer-ul">
                  <div class="ul-title">大数据</div>
                   <ul>
                  
                  
              </ul>
              
              </div>
          </div>
          <div class="footer-r">
              <div class="top">
                <div>
                    <span>

                    </span>
                    <span>
                        BGI·MARINE<br>
                        华大海洋&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
                    </span>
                </div>      
              </div>
              <div class="bottom">
                <div>
                    <div>FAX:0755-36352508</div>
                    <div>TEL:0755-36307296</div>
                    <div>ADD:深圳市盐田区北山工业区136号华大基因11栋</div>
                </div>      
              </div>
          </div>
          <div class="footer-div">
          <span></span>
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
                showText1:false,
                showText2:false,
                showText3:false,
                showText4:false,
                showText5:false,
                showText6:false,
                showText7:false,
                showText8:false,
                showText9:false,
                showText10:false,
                showBall:false,
                showBalls:false,
                showmore:false
            };
        },
        mounted () {
            setInterval(()=>{
                this.num++
                if(this.num>=3){
                    this.num=0
                }
            },500)
            //this.setAnimation()
        },
        methods : {
            showMore(){
                this.showmore = true;
                this.$nextTick(()=>{
                    let height = document.body.clientHeight;
                    for(let i =1;i<=50;i++){
                        setTimeout(()=>{
                             document.body.scrollTop = height*i/50
                        },i*2)
                        
                    }
                    setTimeout(()=>{
                            this.setAnimation()
                        },100)           
                })
                
            },
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
                setTimeout(()=>{
                    for(let i = 1;i<=10;i++){
                        setTimeout(()=>{
                            this["showText"+i] = true
                        },i*600)
                    }
                },3000)  
            }
        }
    }
</script>
<style lang="scss">
.hd-home{
    height: 100%;
    box-sizing: border-box;
    font-family: "宋体";
}
.home-first{
    height: 100%;
    padding-top: 60px;
    background: url("../assets/bg.jpg") no-repeat center center;
    background-size: auto 100%;
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
    background: url(../assets/logo.png) no-repeat left;
    background-size: auto 100%;
    padding-left: 70px;
    display: inline-block;
    margin-left: 480px;
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
    font-size: 14px;
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
    bottom: 20px;
    width: 100%;
    text-align: center;
    color: #aaa;
    line-height: 8px;
    .iconfont{
        font-size: 24px;
        &.light{
            color: #ddd;
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
    animation: opacity 1.5s linear;
  
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
    left: 215px;
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
.tip-top{
    text-align: center;
    font-size: 16px;
}
.center-tips{
    text-align: center;
}
.tips-div{
    height: 1px;
    display: inline-block;
    width: 25px;
    background: #004962;
    margin: 15px 0 0;
}
.tips-c{
    font-size: 18px;
    span{
        transform: scale(.5 ,.5);
        display: inline-block;
        width: 1000px;
    }
}
.center-btns{
    text-align: center;
    padding: 60px;
    span{
        display: inline-block;
        padding: 4px 20px;
        border: solid 1px #666;
        font-size: 14px;
    }
}
.footer{
    background: #0a5b78;
    color: #fff;
    height: 260px;
    padding:0 260px; 
    a{
        color: #fff;
        text-decoration: none;
    }
    position: relative;
}
.footer-ul{
    margin-top: 60px;
    float: left;
    transform: translate(-50px,-25%) scale(.5,.5);
    .ul-title{
        font-size: 18px;
        margin-bottom: 40px;
    }
    ul{
        li{
            list-style: none;
            margin-bottom: 10px;
        }
    }
}
.footer-r{
    position: absolute;
    right: 200px;
    margin-top: 30px;
    text-align: right;
    transform: scale(.5,.5) translate(50%,-25%);
    .top{
        background: url(../assets/logomultiply.png) no-repeat 200px;
    }
    .bottom{
        margin-top: 140px
    }
}
.footer-div{
    position: absolute;
    top: 210px;
    width: calc(100% - 426px);
    left: 226px;
    padding: 0;
    margin: 0;
    span{
        height: 1px;
        display: block;
        background: #fff;
    }
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
				from {opacity: 0;height: 0;}
				to {opacity: 1;height:30px;}
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

