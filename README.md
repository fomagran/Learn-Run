<p>안녕하세요 Foma 입니다!!</p>
<p>&nbsp;</p>
<p>저번 시간에 현재 위치에 대한 권한을 받아오고 현재 위치를 알아보는 방법에 대해서 알아보았는데요.</p>
<p>&nbsp;</p>
<p>혹시라도 못보신 분들은 여기 로 이동하셔서 보고 와주세요~</p>
<p>&nbsp;</p>
<p>오늘은 현재 위치의 날씨와 앞으로의 24시간,앞으로의 일주일간 날씨 데이터를 받아와서 화면에 띄워볼거에요.</p>
<p>&nbsp;</p>
<p>바로 시작할게요~</p>
<hr contenteditable="false" data-ke-type="horizontalRule" data-ke-style="style6" />
<p>Preview</p>
<p>&nbsp;</p>
<p>[##_Image|kage@cfOwt1/btqYhz4ooJB/DfoEsVvJtqzYo8Il6FCS6k/img.png|alignCenter|data-filename="IMG_5081.PNG" data-origin-width="1125" data-origin-height="2436" width="337" height="NaN" data-ke-mobilestyle="widthContent"|||_##]</p>
<hr contenteditable="false" data-ke-type="horizontalRule" data-ke-style="style6" />
<p>Pod</p>
<p>&nbsp;</p>
<p>우선 날씨 데이터를 받아오기 위해서 저는 Alamofire,SwiftyJSON 이라는 라이브러리를 사용했는데</p>
<p>&nbsp;</p>
<p>여러분들도 podfile에 추가하신뒤 pod install 해주세요~</p>
<pre id="code_1613986306926" class="swift" data-ke-language="swift" data-ke-type="codeblock"><code>pod 'SwiftyJSON', '~&gt; 4.0'
pod 'Alamofire', '~&gt; 5.2'</code></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>현재 위치의 날씨</p>
<p>&nbsp;</p>
<p>CurrentWeather</p>
<p>&nbsp;</p>
<p>CurrentWeatehr 클래스를 하나 만들어줍니다.</p>
<p>&nbsp;</p>
<p>도시,날짜,온도,날씨정보를 띄울 변수들을 만들어주세요!</p>
<pre id="code_1613986175421" class="swift" data-ke-language="swift" data-ke-type="codeblock"><code>    var city:String = ""
    var date:String = ""
    var temp:Double = 0.0
    var weatherInfo:String = ""</code></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>WeatherView</p>
<p>&nbsp;</p>
<p>날씨를 띄울</p>
<pre id="code_1613986125347" class="swift" data-ke-language="swift" data-ke-type="codeblock"><code> var currentWeather:CurrentWeather!</code></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>


