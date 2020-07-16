<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>网上登记服务注册平台</title>
    <link rel="shortcut icon" type="image/x-icon" href="img/favicon.ico">
    <link rel="stylesheet" href="css/login.css">
    <script src="./js/jquery.js"></script>
</head>

<body>
    <header class="header">
        <div class="container">
            <div class="logo">
                <img src="./img/国徽.png" style="width: 40px; height: 40px;">
            </div>
            <p>甘肃省工商网上登记注册服务平台</p>

        </div>
        <div class="menu">
            <nav>
                <a href="javascript:;" class="e">
                    <img src="./img/e图标.png">
                    <p>全程电子化</p>
                </a>
                <p>|</p>
                <a href="javascript:;" class="app">
                    <img src="./img/手机小图标.png">
                    <p id="ppp">手机APP</p>
                </a>
                <div class="modal">
                    <img src="" alt="">
                </div>
            </nav>
        </div>


    </header>


    <div class="banner">
        <div class="container clearfix">
            <iframe class="right loginarea" src="infirm.html" frameborder="0"></iframe>
            <div class="left">
                <div class="slogan">
                    <img src="./img/工商登记，从这里开始.png" alt="">
                </div>
                <div class="xu">
                    <img src="./img/虚拟大厅图标.png" alt="">
                    <p>虚拟大厅</p>
                </div>
                <div class="ban">
                    <img src="./img/办理指南图标.png" alt="">
                    <p>办理指南</p>
                </div>
            </div>
        </div>

    </div>

    <!-- 文字 -->
    <div class="tab">
        <div class="container clearfix">
            <ul class="tab-title">
                <li class="this">公示公告</li>
                <li>政策法规</li>
                <li>常见问题</li>
                <li></li>
            </ul>
            <div class="word">

            </div>
        </div>

    </div>

    <!-- 页脚 -->
    <footer class="footer">
        <div class="container clearfix">
            <div class="left">
                <img src="./img/红图标.png" alt="">
            </div>
            <div class="right">
                <p>
                    &nbsp;&nbsp;Copyright 2003-2013 www.xxx.com, All Rights Reserved 甘ICP备00000000号
                    站长统计<br>
                    国内最大的XXXXXXXXXXX网站 电话：400-123-456 地址：甘肃省兰州市城关区XXX号 E-mainl:0000000@qq.com
                </p>
            </div>
        </div>
    </footer>

</body>
<script>
    let ppp = document.getElementById("ppp");
    let modal = document.querySelector('.modal');
    let flag = 0;
    ppp.addEventListener('click', function () {
        if (flag === 0) {
            modal.style.visibility = 'visible';
            flag = 1;
        } else {
            modal.style.visibility = 'hidden';
            flag = 0;
        }
    })
</script>
<script>
    // var 
    $.ajax({
        url: "/greet",
        data: { name: 'jenny',gjagji:'gaga ' },
        type: "POST",
        dataType: "json",
        success: function (data) {
            if (data ===true) {
                location.href= "";
            } else {
                alert('你的XXX不合适');
            }
            // data = jQuery.parseJSON(data);  //dataType指明了返回数据为json类型，故不需要再反序列化

        }
    })
</script>

</html>
