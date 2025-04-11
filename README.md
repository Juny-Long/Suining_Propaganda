
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="绥宁城市宣传网站，让各地人民可以通过网上冲浪详细了解绥宁的介绍、景色、特色、发展及现状，从而提高绥宁的知名度，让更多的人知道绥宁，认识绥宁，来到绥宁，致力于促进绥宁县的经济与生态共同良性发展">
    <meta name="keywords" content="绥宁,绥宁宣传,神奇绿洲,长铺,绥宁介绍,黄桑，寨市">
    <title>注册界面</title>
<!--     <link rel="shortcut icon" href="./images/useR/fx/favicon.ico" type="image/x-icon">
    <link rel="stylesheet" href="./CSS/login.css">
    <script type="text/javascript" src="./JS/time.js"   ></script> -->
   
</head>
    <style>
      .input{
           color: rgb(197, 65, 65);
         border: 1px solid ;
      }
    </style>
    <script  type="text/javascript">   
  
    </script>

<body  style=" background-image:url(./images/ly/img7.jpeg) ;background-size:100%;">
    <form name="form" method="post" action="./login.html" >
<script>
</script>
    <div class="one">
       <h1 >--注册/登录--</h1>
      <Table>
        <TR>
          <td> <b>邮箱：</b></td>
          <td><input type="text" name="email" placeholder="请输入邮箱" id="email"   required> </td>
          <td  id="emailerr"  ></td>
        </tr>
        <tr>
          <td><b>账号：</b></td>
          <td><input type="text" name="account" placeholder="请输入手机号" id="account"  required  > </td>
          <td id="accounterr"></td>
        </tr>
        <tr>
          <td><b>密码：</b></td>
          <td><input type="password" name="pw" placeholder="请输入密码" id="pw" required> </td>
          <td id="pwerr"></td>
        </tr>
          <td><b>确认：</b></td>
          <td><input type="password" name="pwr" placeholder="请确认密码"  id="pwr"  required > </td>
          <td id="pwrerr"></td>
        <tr>
         <td><b>性别：</b></td>
          <td><select id="sex" required >
               <option value="no_sex" name="no_sex" disabled>请选择性别</option>
               <option value="男" name="man" >男</option>
               <option value="女" name="woman" >女</option>
               <option value="保密" name="secrecy" >保密</option>
              </select>
              <label onclick="re_xieyi()"  > <input type="checkbox" class="xianzong" required >  <a href="#xieyi">阅读用户协议</a></label> 
          
                    <div style="display: none;" id="xieyi">
                        <textarea rows="10" cols="30" readonly;>尊敬的客户，欢迎您注册成为绥宁城市宣传网站(以下简称:"本网站")的用户。在注册前请您仔细阅读如下服务条款：
            
                            本服务协议双方为本网站与本网站客户，本服务协议具有合同效力。您确认本服务协议后，本服务协议即在您和本网站之间产生法律效力。请您务必在注册之前认真阅读全部服务协议内容，如有任何疑问，可向本网站咨询。 无论您事实上是否在注册之前认真阅读了本服务协议，只要您点击协议正本下方的"注册"按钮并按照本网站注册程序成功注册为用户，您的行为仍然表示您同意并签署了本服务协议。</textarea>
                      <button disabled onclick="read()" type="button"> 已同意阅读协议(10s)</button>
                    <!-- //防止自动提交,增加 button的 type 为button -->
                    <!-- button除了在IE浏览器的默认类型type是“button”而在其他浏览器中（包括w3c规范）的默认类型type都是“submit”。所以我们应该始终为按钮button规定type属性。 -->
                    </div>
                    <script>
                    //  阅读协议
        let btn=document.querySelector('button')
        var i=10

      function read(){
       // document.getElementById('reg').disabled=false
       document.getElementById('xieyi').style.display="none";
  
       }

       function re_xieyi(){

           document.getElementById('xieyi').style.display="block";
        let time= setInterval(function(){
           i--
               
           if(i===0 || i<0){
               clearInterval(time)
               btn.innerHTML=`同意阅读协议`
               btn.disabled=false
           }else{
             btn.innerHTML=`请同意阅读协议(${i}s)`
           }
          
       },500)
       }
                   </script>
          </td>
        </tr>
       
      </Table>
          <!-- <input type="submit" class="a" value="登录">&nbsp;&nbsp; -->
            <input type="submit"  class="a" di="reg" value="注册" >
            &nbsp;&nbsp;
            <input type="reset"  class="c" value="重置"> 
         <div><p>注：(如若忘记账号，请用e-mail找回账号)&nbsp;
          <a href="./suining index.html" >首页</a><a href="./login.html" >登录</a></p></div>
       
    </div>
    </form>
    <div id="now_time">
        <script type="text/javascript">
            return_time();
        </script>
      </div>
      <!-- <div> <audio src="./muisc/注册页面.mp3" controls  autoplay preload="auto"></audio></div> -->
      <script type="text/javascript" src="./JS/register.js"   ></script>
</body>



</html>
