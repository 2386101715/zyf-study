1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:      <h1 id="h1"></h1>
    <script>
         var h1 = document.getElementById('h1') 
         var str = 'a';
         var str2 = 'b';
         var st3 = str.Concote(str2);
         console.log(st3);
         h1.innerHTML = st3;
    </script>
2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:      var btn = document.getElementById('btn');
			var in1 = document.getElementById('in1');
			//var str = in1.value;
			btn.onclick = function(){
				var str = in1.value;
				if(str.length<8){
					var sstr = str.padEnd(6,'0');
                    console.log(sstr);
				}else{
					alert("存款失败");
				}  
			}
3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:   <h3 id="h3"></h3>
    <script>
      var h3 = document.getElementById('h3') 
      var str = '79387.348';
      var ste = str.substr(0,8);
      console.log(ste);
      h3.innerHTML = ste;
    </script>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:     <img src="img/head/icon/1.jpg" id="img"/>
		<h4 id="h4"></h4>
		<script type="text/javascript">
			var img=document.getElementById("img");
			var h4=document.getElementById("h4");
			h4.innerHTML=img.src;
        </script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:     var s1 = 'ABCSJ'
        var s2 = 'abcsj'
        console.log(s1.toLowerCase());
        console.log(s2.toUpperCase());