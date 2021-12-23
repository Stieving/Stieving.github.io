<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://kit.fontawesome.com/2b5583f7d5.js" crossorigin="anonymous"></script>
    <link rel="stylesheet" href="css/style.css">
    <link href='https://fonts.googleapis.com/css?family=Nosifer' rel='stylesheet'>
    <link href='https://fonts.googleapis.com/css?family=Monsieur La Doulaise' rel='stylesheet'>
    <script src="js/main.js"></script>
    <title>Tryboks:Reloaded</title>

    <style>
        .showcase .showcase-content>h1 {
            font-family: 'Nosifer';
            font-size: 50px;
        }
        
        .trailer_h2 {
            font-family: 'Monsieur La Doulaise';
            font-size: 50px;
            text-align: center
        }
    </style>

</head>

<body onload="onload();">
    <header class="showcase">
        <div class="showcase-content">
            <h1>TRYBOKS: RELOADED</h1>
        </div>
    </header>

    <p class="coming-soon"><i>Coming soon...</i></p>

    <section class="tabs">
        <div class="container">
            <div id="tab-2" class="tab-item">
                <i class="fas fa-film fa-3x">                 
                </i>
                <p class="hide-sm">Watch Trailer</p>
            </div>
    </section>

    <video id="idle_video" width="1100" height="400" onended="onVideoEnded();" controls autoplay muted></video>
    <script>
        var video_list = ["/vid/VID-20211214-WA0014.mp4",
            "/vid/VID-20211214-WA0016.mp4",
            "/vid/VID-20211215-WA0038.mp4",
            "/vid/VID-20211215-WA0039.mp4"
        ];
        var video_index = 0;
        var video_player = null;

        function onload() {
            console.log("body loaded");
            video_player = document.getElementById("idle_video");
            video_player.setAttribute("src", video_list[video_index]);
            video_player.play();
        }

        function onVideoEnded() {
            console.log("video ended");
            if (video_index < video_list.length - 1) {
                video_index++;
            } else {
                video_index = 0;
            }
            video_player.setAttribute("src", video_list[video_index]);
            video_player.play();
        }
    </script>

    <h2 class="trailer_h2"> This is just the beginning</h2>



    <!--Tab 1 Content-->
    <div id="tab-1-content" class="tab-content-item">
        <div class="tab-1-content-inner">
            <div>
                <p class="text-lg" style="text-align: center;">
                    Meet the <i>JAG</i>
                </p>
            </div>

            <div class="grid">
                <img src="/img/IMG-20210730-WA0010.jpg" alt="">
                <img src="/img/IMG-20210730-WA0022.jpg" alt="">
                <img src="/img/IMG-20210822-WA0041.jpg" alt="">
                <img src="/img/IMG-20210916-WA0057.jpg" alt="">
                <img src="/img/IMG-20210918-WA0028.jpg" alt="">
                <img src="/img/IMG-20210918-WA0020.jpg" alt="">
                <img src="/img/IMG-20210918-WA0021.jpg" alt="">
                <img src="/img/IMG-20210918-WA0034.jpg" alt="">
            </div>

        </div>


    </div>



    <!-- 3rd content -->

    <div id="tab-3-content" class="tab-content-item">
        <div>
            <h1>Behind The Scenes</h1>
        </div>
        <div class="tab-3-content-top grid">
            <img src="/img/imgg/IMG-20210724-WA0042.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0043.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0045.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0047.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0048.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0049.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0050.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0051.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0052.jpg" alt="">
            <img src="/img/imgg/IMG-20210724-WA0053.jpg" alt="">
        </div>
        <div class="tab-3-content-bottom btn btn-icon">
            <a href="#">www.tryboks.com/officialthemesong</a>
        </div>
        <div class="tab-3-content-bottom btn btn-icon">
            <a href="#">www.trybok.com/characters</a>
        </div>
    </div>

    <footer class="footer">
        <p>Questions? Call 1-866-579-7172</p>
        <div class="footer-cols">
            <ul>
                <li><a href="#">TRYBOKS Originals</a></li>
                <li><a href="#">Ways To Watch</a></li>
                <li><a href="#">FAQ</a></li>
            </ul>
            <ul>
                <li><a href="#">Help Center</a></li>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
            <ul>
                <li><a href="#">Privacy</a></li>
                <li><a href="#">Cookie Preferences</a></li>
                <li><a href="#">Legal Notices</a></li>
            </ul>
        </div>
    </footer>


</body>

</html>
