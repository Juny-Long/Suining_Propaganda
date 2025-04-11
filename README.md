<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="绥宁城市宣传网站，让各地人民可以通过网上冲浪详细了解绥宁的介绍、景色、特色、发展及现状，从而提高绥宁的知名度，让更多的人知道绥宁，认识绥宁，来到绥宁，致力于促进绥宁县的经济与生态共同良性发展">
    <meta name="keywords" content="绥宁,绥宁宣传,神奇绿洲,长铺,绥宁介绍,黄桑，寨市">
    <title>登录界面</title>
    <link rel="shortcut icon" href="./images/useR/fx/favicon.ico" type="image/x-icon">
    <link rel="stylesheet" href="./CSS/login.css" type="text/css">
    <script type="text/javascript" src="./JS/time.js"></script>
</head>
<style>
        
</style>

<body style=" background-image:url(./images/ly/img7.jpeg) ;background-size:100%;">
    <form action="user.html" method="post">
        <div class="one">
            <h1>--注册/登录--</h1>
            <b>账号：</b><input type="text" name="account" placeholder="请输入手机号" id="account"
                 required><span id="accounterr"></span></br>
            <b>密码：</b><input type="password" name="pw" placeholder="请输入密码" id="pw"
                required><span id="pwerr"></span></br>
            <input type="submit" class="a" value="登录" onclick=" return login()">&nbsp;&nbsp;
            <input type="reset" class="c" value="重置">
            <div>
                <p>注：(如若忘记账号，请用e-mail找回账号)&nbsp;<a href="./suining index.html">首页</a><a href="./register.html">注册</a>
                </p>
            </div>
        </div>
    </form>
    <div id="now_time">
        <script type="text/javascript">
            return_time();
        </script>
    </div>
    <script type="text/javascript" src="./JS/login.js"></script>
</body>

</html>
