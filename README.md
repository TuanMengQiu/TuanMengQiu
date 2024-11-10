### 团梦秋介绍
 > 2018年自学触发器取得成功，2020年制作第一期触发器教学视频2021年3月学习C语言并尝试制作迷你世界脚本，2021年7月份在虎牙开始第一次直播，累计粉丝936个，萌新主播一枚，2022年2月33号自研防G脚本1.0制作完成，2022年8月1号在胖柴发布了防G脚本0.5供所有玩家下载
 > 
 > 曾用别称<梦飝游戏解说><团梦秋游戏解说><团梦秋><喜哒-团梦秋><知卿-团梦秋>
### 保险箱防护插件包
![](https://tuanmengqiu.cn/studio/bxxfh/img/icon.png)
> 保险箱防护插件包是由梦秋工作室成员团梦秋制作的被动防御插件包
>
> 插件包专门解决保险箱能被拆、利用bug刷物品、利用bug卡房问题
>
> 下方为资源工坊id
> ``` 资源工坊id
> 636968783_1726561015
> ```
>
> 点击[查看更新公告](https://tuanmengqiu.cn/studio/bxxfh/)

### 加入梦秋工作室
> 工作室QQ群:923032296
>
> 点击[加入工作室](https://qm.qq.com/q/NLOSp2JjeU)



<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="utf-8">
    <title>团梦秋赛事</title>
    <link rel="shortcut icon" href="https:\\tuanmengqiu.cn\static\picture\a4Vyng.jpg" type="image/x-icon">
    <link rel="bookmark" href="https:\\tuanmengqiu.cn\static\picture\a4Vyng.jpg">
    <link href="static/css/qiuqiu.css" rel="stylesheet" type="text/css">
    <link href="static/css/styles.css" rel="stylesheet">
        <style>
        .lbt {
            margin: 0;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 450vh;
        }
        .outer-shell {
            position: relative;
            width: 90%;
            max-width: 1000px;
            padding: 20px;
            background-image: url('https://tuanmengqiu.cn/cx/img/bj.png'); /* 外壳背景图片 */
            background-size: cover;
            background-position: center;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .slider {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
        }

        .slides {
            display: flex;
            transition: transform 0.6s ease-in-out;
        }

        .slides img {
            width: 100%;
            height: auto;
            border-radius: 10px;
        }

        button {
            position: absolute;
            top: 50%;
            background-color: rgba(0, 0, 0, 0.6);
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            font-size: 24px;
            border-radius: 50%;
            transform: translateY(-50%);
            transition: background-color 0.3s ease;
            z-index: 10;
        }

        button:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }

        .prev {
            left: 10px;
        }

        .next {
            right: 10px;
        }

        .dots {
            text-align: center;
            position: absolute;
            bottom: 15px;
            width: 100%;
            display: flex;
            justify-content: center;
            gap: 10px;
            z-index: 10;
        }

        .dot {
            display: inline-block;
            width: 12px;
            height: 12px;
            background-color: #bbb;
            border-radius: 50%;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .dot.active {
            background-color: #717171;
        }
        
    </style>
</head>
<body>
    <div class="lbt">
        <div class="outer-shell">
        <div class="slider">
            <div class="slides">
                <img src="images/image1.jpg" alt="Image 1">
                <!-- 可以继续添加更多图片 -->
            </div>
            <button class="prev">‹</button>
            <button class="next">›</button>
            <div class="dots">
                <span class="dot"></span>
                <span class="dot"></span>
                <span class="dot"></span>
                <!-- 根据图片数量调整点的数量 -->
            </div>
        </div>
    </div>
</div>
    <script>
        const slides = document.querySelector('.slides');
        const images = document.querySelectorAll('.slides img');
        const dots = document.querySelectorAll('.dot');
        let index = 0;
        let interval;

        function showSlide(n) {
            if (n >= images.length) {
                index = 0;
            } else if (n < 0) {
                index = images.length - 1;
            } else {
                index = n;
            }
            slides.style.transform = `translateX(${-index * 100}%)`;
            updateDots();
        }

        function updateDots() {
            dots.forEach((dot, i) => {
                dot.classList.toggle('active', i === index);
            });
        }

        function startAutoSlide() {
            interval = setInterval(() => {
                showSlide(index + 1);
            }, 3000); // 每3秒自动切换
        }

        function stopAutoSlide() {
            clearInterval(interval);
        }

        document.querySelector('.next').addEventListener('click', () => {
            showSlide(index + 1);
            stopAutoSlide(); // 点击按钮时停止自动轮播
            startAutoSlide(); // 重新启动自动轮播
        });

        document.querySelector('.prev').addEventListener('click', () => {
            showSlide(index - 1);
            stopAutoSlide(); // 点击按钮时停止自动轮播
            startAutoSlide(); // 重新启动自动轮播
        });

        dots.forEach((dot, i) => {
            dot.addEventListener('click', () => {
                showSlide(i);
                stopAutoSlide(); // 点击点时停止自动轮播
                startAutoSlide(); // 重新启动自动轮播
            });
        });

        // Initial setup
        showSlide(index);
        startAutoSlide();
    </script>
    
        <div class="part part6" id="page6">
            <div class="part6-con">
                <div class="part6-li">
                    <a href="https://www.huya.com/27644739" target="_blank">
                    <img src="static/picture/code-hy.png">
                    <p>虎牙直播</p>
                    </a>
                </div>
                <div class="part6-li">
                    <a href="https://space.bilibili.com/1447502167" target="_blank">
                    <img src="static/picture/code-bl.png">
                    <p>哔哩哔哩</p>
                    </a>
                </div>
                <div class="part6-li">
                    <a href="https://www.ixigua.com/home/607360094052119" target="_blank">
                    <img src="static/picture/code-xg.png">
                    <p>西瓜视频</p>
                    </a>
                </div>
                <div class="part6-li">
                    <div class="qq-link">
                        <a href="http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=7XMNoKnFRK-g6h9JRGLXAsxIST7O1gpj&authKey=cNo0LMLOanR%2FUimIfgcIedpGfGheVcRJOYrVTUfBNURLWxdvWH3Kq0fnkUG05xTr&noverify=0&group_code=124605944"target="_blank" onclick="PTTSendClick('btn','link1','迷你比赛群');">124605944</a>
                    </div>
                    <p>比赛QQ群</p>
                </div>
            </div>
        </div>




    <div class="copyright">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <p style="color: #dfe5ec;margin-bottom:0rem">团梦秋微赛事</p>
                    <p class="p-small">Copyright &copy; 2024 <a href="https://tuanmengqiu.cn/"target="_blank"</a>梦秋工作室MengQiu Studio</a><!--丨--><a href="https://beian.miit.gov.cn/" target="_blank" rel="noreferrer"><!--ICP备案：吉xxxxxx号-x--></a></p>
                </div> <!-- end of col -->
            </div> <!-- enf of row -->
        </div> <!-- end of container -->
    </div> <!-- end of copyright --> 
    <!-- end of copyright -->
    <!-- Scripts -->

    <!--鼠标样式-->
    <img class="mouse" src="img/logo.png" alt="">
    <script src="static/js/mouse.js"></script>
    <link href="static/css/mouse.css" rel="stylesheet">

    <!--网页黑白-->
  <!--
    <link href="static/css/heibai.css" rel="stylesheet">
  -->
    <script src="static/js/huaban.js"></script><!--花瓣效果-->
<audio src="static/picture/1.mp3" loop="loop" autoplay="autoplay"></audio>
</body>
</html>

