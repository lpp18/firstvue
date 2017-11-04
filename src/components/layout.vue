<template>
 <div>
    <div class="app-head">
      <div class="app-head-inner">
        <img src="../assets/logo.png" alt="">
        <div class="head-nav">
          <ul class="nav-list">
            <li>登录</li>
            <li class="nav-plie">|</li>
            <li>注册</li>
            <li class="nav-plie">|</li>
            <li>关于</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="app-content">
    <keep-alive>
       <router-view></router-view>
    </keep-alive>

    </div>
    <div class="app-footer">
      <p>© 2016 fishenal MIT</p>
    </div>
 </div>
</template>

<script>
   export default{
    data(){
      return {
      msg:'i am apple',
      price:5
      }
    }
   }
</script>
<style>
  body, h1, h2, h3, h4, h5, h6, hr, p, blockquote, dl, dt, dd, ul, ol, li, pre, form, fieldset, legend, button, input, textarea, th, td { margin:0; padding:0; }
  body, button, input, select, textarea { font:12px/1.5tahoma, arial, \5b8b\4f53; }
  h1, h2, h3, h4, h5, h6{ font-size:100%; }
  address, cite, dfn, em, var { font-style:normal; }
  code, kbd, pre, samp { font-family:couriernew, courier, monospace; }
  small{ font-size:12px; }
  ul, ol { list-style:none; }
  a { text-decoration:none; }
  a:hover { text-decoration:underline; }
  sup { vertical-align:text-top; }
  sub{ vertical-align:text-bottom; }
  legend { color:#000; }
  fieldset, img { border:0; }
  button, input, select, textarea { font-size:100%; }
  table { border-collapse:collapse; border-spacing:0; }

  .app-head{
    padding-left:10px;
    padding-right:10px;
    height:50px;
    background: rgba(0,0,0,.7)
  }
  .app-head-inner{
    height: 100%;
    display: flex;
    justify-content: space-between;
    vertical-align:middle;
    align-items: center;
  }
  .app-head-inner img{
    width:30px;
    height:30px;

  }
  .nav-list{
    height:100%;
    display: flex;
    flex-direction: row;
    align-items: center;
  }
  .nav-plie{
    margin-left:10px;
    margin-right:10px;
  }
  .nav-list li{
     color:#aaa;
  }
  .app-footer{
    height:80px;
    background: #ddd;

  }
  .app-footer p{
    height:80px;
    text-align: center;
    font-size:15px ;
    line-height: 80px;
  }
</style>
