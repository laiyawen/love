<!DOCTYPE HTML>
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		<title>Our Story -- 两天的博客</title>
		<meta name="description" content="两天的博客，记录生活点滴。我只有两天，我从没有把握，一天用来希望，一天用来绝望。" />
		<meta name="keywords" content="两天,平男,博客,田野,田成锋,两天的博客,HTML5表白" />
	<meta http-equiv="content-type" content="text/html; charset=UTF-8">
	<style type="text/css">
		@font-face {
			font-family: digit;
            src: url('font/digital-7_mono-webfont.eot');
            src: url('font/digital-7_mono-webfont.eot?#iefix') format('embedded-opentype'),
                 url('font/digital-7_mono-webfont.woff') format('woff'),
                 url('font/digital-7_mono-webfont.ttf') format('truetype'),
                 url('font/digital-7_mono-webfont.svg#digital-7mono') format('svg');

		}
		@font-face {
			font-family: enword;
			src: url('font/Note_this.ttf') format("truetype");
		}
		@font-face {
			font-family: cnword;
			src: url('font/senty.ttf') format("truetype"),
		      url('font/senty.eot?#iefix') format('embedded-opentype');
		}
	    @font-face {
			font-family: angelina;
			src: url('font/angelina.ttf') format("truetype"),
		         url('font/angelina.eot') format("opentype");
		}
		
	</style>
	<link rel="shortcut icon" href="http://216.127.180.163/favicon.ico" />
	<link href="css/default_dev.css" type="text/css" rel="stylesheet">
	<script type="text/javascript" src="js/jquery.js"></script>
	<script type="text/javascript" src="js/garden.js"></script>
    <script type="text/javascript" src="js/functions_dev.js"></script>
    <script type="text/javascript" src="js/console.js"></script>
</head>

<body>

	<div id="mainDiv">
		<div id="content">
		
			<div id="code">
                <span class="comments center">班扎古鲁白玛的沉默</span>
                <span class="comments center">--扎西拉姆·多多</span>
                <span class="comments">你见，或者不见我 </span>
                <span class="comments">我就在那里 </span>
                <span class="comments">不悲不喜 </span>
                <span class="comments">你念，或者不念我 </span>
                <span class="comments">情就在那里</span>
                <span class="comments">不来不去</span>
                <span class="comments">你爱，或者不爱我 </span>
                <span class="comments">爱就在那里 </span>
                <span class="comments">不增不减</span>
                <span class="comments">你跟，或者不跟我 </span>
                <span class="comments">我的手就在你手里 </span>
                <span class="comments">不舍不弃 </span>
                <span class="comments">来我的怀里 </span>
                <span class="comments">或者 </span>
                <span class="comments">让我住进你的心里 </span>
                <span class="comments">默然 相爱 </span>
                <span class="comments">寂静 欢喜</span>
                </div>

			<div id="loveHeart">
				<canvas id="garden"></canvas>
				<div id="words">
					<div id="messages">
						ZhenZhen, I have met you for
						<div id="elapseClock"></div>
					<div class="loveupersec">The clock rotation for a second.<br />I will love one more second.</div>
					
					</div>

					<div id="loveu">
					
						Love you...<br/>
						<div class="signature">- T.D.</div>
					</div>
				</div>
			</div>
		</div>
		<div id="copyright">
			Copyright © 2014 <a target='_blank' href='http://2days.org'>T.D.</a>
      <br/>
浏览<script src="http://count.2881.com/count/count.asp?id=56758&sx=1&ys=42" language="JavaScript" charset="gb2312"></script>次。

		</div>
	</div>
<audio id="myaudio" loop>
  <source src="./sound/click.mp3" type="audio/mpeg" />
</audio>
	<script type="text/javascript">
		var offsetX = $("#loveHeart").width() / 2;
		var offsetY = $("#loveHeart").height() / 2 - 55;
		var together = new Date();
		together.setFullYear(2014, 11, 05);  //时间年月日（注意月份是从0开始的）
		together.setHours(20);
		together.setMinutes(0);
		together.setSeconds(0);
		together.setMilliseconds(0);
		
		if (!document.createElement('canvas').getContext) {
			var msg = document.createElement("div");
			msg.id = "errorMsg";
			msg.innerHTML = "Your browser doesn't support HTML5!<br/>Recommend use Chrome 14+/IE 9+/Firefox 7+/Safari 4+"; 
			document.body.appendChild(msg);
			$("#code").css("display", "none")
			$("#copyright").css("position", "absolute");
			$("#copyright").css("bottom", "10px");
		    document.execCommand("stop");
		} else {
			setTimeout(function () {
				startHeartAnimation();
			}, 1000);

			timeElapse(together);
			setInterval(function () {
				timeElapse(together);
			}, 500);

			adjustCodePosition();
			$("#code").typewriter();
		}

	</script>
<embed src="http://www.xiami.com/widget/442076_1770542657,_1_1_cccccc_dddddd_1/multiPlayer.swf" type="application/x-shockwave-flash" width="1" height="1" wmode="opaque"></embed>

</body>
</html>
