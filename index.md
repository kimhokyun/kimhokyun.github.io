<!DOCTYPE html> 
<html> 
<head> 
	<title>My Blog </title> 
</head> 
<!-- css 스타일 -->
<style> 
/*html 속성 */
	html {
		font-family:"Source Sans Pro";
		position: relative;
	}
	hr { 
		border : 0;
		height: 1px;
	}
	h1 { 
		display: block;
		font-size: 2.5em;
		margin-top: 0em;
		margin-bottom: 0.3em;
		margin-left: 0;
		margin-right: 0;
		text-align: center;
	}
	h2 { 
		display: block;
		font-size: 1.5em;
		margin-top: 0em;
		margin-bottom: 0.67em;
		margin-left: 0;
		margin-right: 0;
		text-align: center;
	}
	h3 { 
		display: block;
		font-size: 1.0em;
		font-weight: lighter;
		margin-top: 0em;
		margin-bottom: 0.67em;
		margin-left: 0;
		margin-right: 0;
		text-align: center;
	}
	img {
		vertical-align: bottom;
	}
	fieldset{
			margin-top: 3%;
			margin-bottom: 3%;
			margin-left: 20%;
			margin-right: 20%;
	}
	#footer_icon{
		width: 18px !important;
		height: 18px !important;
	}

/* 갤러리 */
	#gallery_pic {
	  width: auto;
	  margin-left : 7%;

	  background: none;
	  box-shadow: 0 1px 2px rgba(0,0,0,.3);
	}

	#gallery_pic > div {
	  position: relative;
	  float: left;
	  padding: 5px;
	  width: 25%;
	}

	#gallery_pic > div > img {
	  display: block;
	  width: 100%;
	  height: auto;
	  transition: .1s transform;
	  transform: translateZ(0);
	  display : table;
	}

	#gallery_pic > div:hover {
	  z-index: 1;
	}

	#gallery_pic > div:hover > img {
	  transform: scale(1.7,1.7);
	  transition: .3s transform;
	}


/* 애니메이션 */
	@-webkit-keyframes example {
		from {opacity:0.6;}
		to {opacity:1;}
	}
/*페이지 레이아웃 */
	#header { 
		background-color: none ; 
		opacity :0.2;
		width: 100%; 
		height: 70px; 
	} 
	#nav { 
		width: 100%; 
		background-color: black; 
		height: auto; 
		opacity:0.6;
		position : fixed;
	}
	#main { 
		width: 100%; 
		background-color: none; 
		color : white;
		float: left; 
		height:637px;
		background: url("용산구.jpg") no-repeat;
		-webkit-background-size: cover;
		background-size: cover;
		-webkit-animation-name: example; /* Safari 4.0 - 8.0 */
		-webkit-animation-duration:2s; /* Safari 4.0 - 8.0 */
	}
	#usadan {
		width: 50%; 
		background-color: none;
		float: left; 
		height: 497px; 
		border: 1px solid white;
		margin-top: 10%;
		margin-bottom: 2%;
		margin-left: 25%;
		margin-right: 25%;
		padding-top: 1em;
		padding-bottom: 0em;
		padding-left: 1em;
		padding-right: 1em;
	}
	#black_bg {
		width: auto; 
		height: 100%; 
		background-color: black;
		opacity : 0.6; 
	}
	#about { 
		width: 99.6%; 
		background-color: none; 
		float: left; 
		height:auto;
		background: url("#.jpg") no-repeat;
		-webkit-background-size: cover;
		background-size: cover;
		-webkit-animation-name: example; /* Safari 4.0 - 8.0 */
		-webkit-animation-duration:2s; /* Safari 4.0 - 8.0 */
		border: solid 1px rgba(160, 160, 160, 0.3);
	}
	#place{ 
		width: 100%; 
		float: left; 
		height:auto;
		width : auto;
		padding-top: 3%;
		padding-bottom: 3%;
		padding-left: 10%;
		padding-right: 10%;
		background-color: rgb(244, 244, 244);
	}
	#GALLERY { 
		width: 80%; 
		background-color: none; 
		float: left; 
		height:auto;
		padding-top: 3%;
		padding-bottom: 3%;
		padding-left: 10%;
		padding-right: 10%;
		background-color: rgb(244, 244, 244); 
		border-bottom: solid 1px rgba(160, 160, 160, 0.3);
	}
	#contact { 
		width: 100%; 
		background-color: black; 
		float: left; 
		height:637px;
		background: url("#.jpg") no-repeat;
		-webkit-background-size: cover;
		background-size: cover;
		-webkit-animation-name: example; /* Safari 4.0 - 8.0 */
		-webkit-animation-duration:2s; /* Safari 4.0 - 8.0 */
		padding-top: 10%;
		padding-bottom: 3%;
		padding-left: 00%;
		padding-right: 00%;
	}
	#contact_sheet {
		width: 50%; 
		background-color: none;
		float: left; 
		height: 497px; 
		border: 1px solid black;
		margin-top: 10%;
		margin-bottom: 2%;
		margin-left: 25%;
		margin-right: 25%;
		padding-top: 1em;
		padding-bottom: 0em;
		padding-left: 1em;
		padding-right: 1em;
	}
	#aside { 
	width: 50%; 
	background-color: gray; 
	float: left; 
	height: 637px; 
	}
	#aside_medium { 
	width: 39%; 
	background-color: white; 
	float: left; 
	height: 497px; 
	padding-top: 0%;
	padding-bottom: 2%;
	padding-left: 0%;
	padding-right: 0%;
	border: solid 1px rgba(160, 160, 160, 0.3);
	}
	#aside_slim { 
	width: 20%; 
	background-color: none;
	opacity :0.2; 
	float: left; 
	height: 497px; 
	}
	#vertical_half{ 
	width: 100%; 
	background-color: gray; 
	float: left; 
	height: 318.5px; 
	}
	#place_pic{
	width: 100%;
	}
	}
/* Footer */
	#footer {
	background-color: black; 
	width: 100%; 
	height: 10%;
	opacity 0.6;
	clear: both;
} 
	#footer > ul {
	background-color: black; 
	color :gray;
	width: auto; 
	height: 100px;
	opacity 0.6;
	clear: both;
	padding-top: 2%;
	padding-bottom: 0%;
	padding-left: 40%;
	padding-right: 40%;
} 
	#footer a:hover {
	color: white;
}
/*네비게이션 바 */
	ul {
		list-style:none;
		text-align:none;
		float:left;
		padding-right: 3%;
	}
	ul li {
		display:inline;
		float : center;
	}
		ul li a { text-decoration:none; color:gray; }
		ul li a:hover { text-decoration:none; color:white; }
</style>
<body style="padding:0px;margin:0px;width:100%;height:100%;"><!-- body 여백 없애기-->
	<div id="wrapper"> 
		<div id="main">
			<div id="black_bg">
				<div id = "usadan">
					<br>
					<hr color=white width=70px>
					<h1>월간우사단</h1>
					<hr color=white width=70px>
					<h3>서울의 중심 이태원 뒷골목, 그 문화와 풍류의 중심 주변 언저리에 위치한
					<h2>"그냥 동네"
				</p><img src = "angle-down.png">
					<br><br><br>
					<hr color=white width=30%>
					<h3>The Monthly x 4 woosadan</h3>
					<h3>2017.10.13 Thursday</h3>
					<h3>제 1 쇄</h3>
				</div>
			</div>
		</div>
		<div id="about">
			<h1> "ABOUT" </h1>
			<b>
			<audio controls loop autoplay="autoplay">
				<source src="bgm.mp3" type="audio/mpeg">
			</audio>
			<fieldset>
			<legend>들어가며</legend>
			월간우사단은 완벽하지는 않지만 작정하고 우리 마을을 전해본다. 동네 어르신들게 들었던 옛 이야기와 최근의 모습을 통해 더 많은 이야기를 나눌 수 있기를 기대한다.
			<br><br>
			사람들 입에 오르내리는 '부자 동네' 중 단연 최고는 아마도 대한민국 재벌들의 저택이 몰려있는 한남동일 것이다. 그러나 한남동을 말할 때 재벌들의 이야기만 나눌수는 없다. 언론과 방송이 말하지 않는 한남동의 이면에는 다문화와 근현대사, 사람 사는 이야기가 숨어있다.
			<br><br>
			한남동의 다문화는 현재 사회적으로 통용되는 다국적 문화가 아니다. 단순한 뜻의 '다양한 문화'로 각기 다른 문화가 공존하는 문화형태를 말한다. 한남동에는 이곳, 저곳 혼재되어있는 부촌과 빈촌으로 인해 형성된 생활문화와 젊은 예술인들의 주목과 관심을 받으며 성장하는 문화, 미군을 비롯한 여러 나라의 외국인들이 모여 만들어낸 문화들이 공존하고 있다.
			</fieldset>
			</b>
			</div>
		</div>
		<div id="place" >
			<h1> [PLACE] </h1>
			<div id="aside_medium"> 
				<img id = "place_pic" src="pic/islam.jpg">
				<h2><br></h2>
				<h2>이슬람 사원</h2>
				<hr color=black width=70%>
				<hr>
				<b>
				<h3>"1974년 제 1차 석유파동으로 경제위기에 몰린 박정희 정권의 이슬람교 포용정책에 의해 1976 이슬람 성원이 생겼다. 처음에는 청파동에 지어지려 했던 이슬람 사원은, 1층은 개인 집이 있고 2층은 학교가 있떤 이광중학교와 터를 맞바꾸었다. 현재 이슬람 성원 부근은 뉴타운 3구역으로 지정되어 있다."
				</b>
			</div>
			<div id="aside_slim"></div>
			<div id="aside_medium">
				<img id = "place_pic" src="pic/market.jpg"> 
				<h2><br></h2>
				<h2>도깨비 시장</h2>
				<hr color=black width=70%>
				<hr>
				<b>
				<h3>"마을에서 가장 높은 능선에 위치한 도깨비시장은 현재 그 자취가 한광교회 인근으로 많이 줄어들었지만 이태원 계단장, 들어와 가게 등으로 다시 그 폭이 넓어지고 있는 추세이다. 산비탈에 위치해 있지만 이태원 역과 가깝고 마을버스가 지나는 길, 우사단로의 도깨비시장은 과거에는 북적거리는 시장이었으나 시간이 흐름에 따라 쇠퇴하였다."
				</b>
			</div>
		</div>
		<div id="GALLERY">
			<h1>[GALLERY]</h1>
			<div id="gallery_pic">
			  <div>
				<img src="pic/1.jpg">
			  </div>
			  <div>
				<img src="pic/2.jpg">
			  </div>
			  <div>
				<img src="pic/3.jpg">
			  </div>
			  <div>
				<img src="pic/4.jpg">
			  </div>
			  <div>
				<img src="pic/5.jpg">
			  </div>
			  <div>
				<img src="pic/6.jpg">
			  </div>
			  <div>
				<img src="pic/7.jpg">
			  </div>
			  <div>
				<img src="pic/8.jpg">
			  </div>
			  <div>
				<img src="pic/9.jpg">
			  </div>  
			  <div>
			  </div>
			 <div>
				<img src="pic/10.jpg">
			  </div> 		
			  <div>
				<img src="pic/11.jpg">
			  </div>
			  <div>
				<img src="pic/12.jpg">
			  </div>
			  <div>
				<img src="pic/13.jpg">
			  </div>
			  <div>
				<img src="pic/14.jpg">
			  </div>
			  <div>
				<img src="pic/15.jpg">
			  </div>
			  <div>
				<img src="pic/16.jpg">
			  </div>
			  <div>
				<img src="pic/17.jpg">
			  </div>
			  <div>
				<img src="pic/18.jpg">
			  </div>
			  <div>
				<img src="pic/19.jpg">
			  </div>
			  <div>
				<img src="pic/20.jpg">
			  </div>
			  <div>
				<img src="pic/21.jpg">
			  </div>
			  <div>
			  </div>
			  <div>
				<img src="pic/22.jpg">
			  </div>
			  <div>
				<img src="pic/23.jpg">
			  </div>
			  <div>
				<img src="pic/24.jpg">
			  </div>
			</div>
		</div>
		<div id="contact">
			<h1>[CONTACT]</h1>
			<div id="contact_sheet">
				<h3><b>CONTACT SHEET</b></h3>
				<il>
					<li>MOBILE : 01098820722</li>
					<li>EMAIL : cjswoghrbs@gmail.com</li>
					<li>ADRRESS : 72-XX, Bogwang-ro, Yongsan-gu, Seoul, Republic of Korea</li>
				</il>
				<br><br><br>
				<form>	
					PRIVACY BOUND
					<input type="radio" name="a" value="a1">public
					<input type="radio" name="a" value="a2">secret
					<br><br><br>
					NAME:  <input type="text" name="name"size=10><br>
					EMAIL: <input type="password" name="pass" size=10>
					@<select name="option">
						<option value="c1"selected>gmail.com</option>
						<option value="c2">naver.com</option>
						<option value="c3">daum.net</option>
						<option value="c4">hanmail.net</option>
					</select>
				<br><br>WORDS <textarea rows="5" cols="40">
				</textarea>
					<input type="submit" value="SUBMIT" />
					<input type="reset" value="RESET" />
				</form>
				</div>
			</div>
		</div>
		<footer id="footer">
			<ul>
				<li><a href="#"><img id="footer_icon" src= "icon\twitter_icon.png">Twitter</a></li>
				<li><a href="#"><img id="footer_icon" src= "icon\facebook_icon.png">Facebook</span></a></li>
				<li><a href="#"><img id="footer_icon" src= "icon\instagram_icon.png">Instagram</span></a></li>
				<li><a href="#"><img id="footer_icon" src= "icon\gmail_icon.png">Email</span></a></li>
			<br><center>&copy; Untitled. All rights reserved.
			</ul>
		</footer> 
		<div id="nav" >
			<ul>
				<li><a href="#main">HOME</a></li>
			</ul>
			<ul style="float:right;"><!--오른쪽 정렬하기 위해 별도로 스타일 지정-->
				<li><a href="#about">ABOUT</a></li>
				<li><a href="#place">PLACE</a></li>
				<li><a href="#GALLERY">GALLERY</a></li>
				<li><a href="#contact">CONTACT</a></li>
			</ul>
		</div> 
	</div> 
</body> 
</html>
