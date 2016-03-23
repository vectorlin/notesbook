# notesbook
<!--hello world-->
<head>
<meta charset="utf-8">
<title>My first GitHub Repository</title>
</head>
<body>
  <h1>Hello World</h1>
  <p>How are you?</p>
  <p>Fine,thank you!</p>
  <p>Happy New Year</p>
  jquery-1.11.3
  easyui
  spss
  highcharts.js
  jquery-easyui-1.3.1
  jquery-easyui-1.3.5
  uploadify-3.1
  cude.js
  juqery.ui
  <br>
  ——3.21
  <br>
  @*  这中间的内容是注释，这是Razor语法，适用于razor语法页面，比如常见的*.cshtml  *@
  <br>
  Jquery插件 easyUI属性汇总 http://www.jb51.net/article/26077.htm
  <br>
  ——3.22
  <br>
  13款实用的JS插件&前端资源 https://www.shiyanlou.com/questions/3524
  <br>
  淘宝前端团队http://taobaofed.org/
  <br>
  ——3.33
  <code>
    <!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>test switch</title>
	<style type="text/css">
*,
*::before,
*::after {
  box-sizing: border-box;
}
.toggle {
  display: block;
  text-align: center;
  margin-top: 40px;
  user-select: none;
}

.toggle--checkbox {
  display: none;
}

.toggle--btn {
  display: block;
  margin: 0 auto;
  font-size: 1.4em;
  transition: all 350ms ease-in;
}
.toggle--btn:hover {
  cursor: pointer;
}

.toggle--btn, .toggle--btn:before, .toggle--btn:after,
.toggle--checkbox,
.toggle--checkbox:before,
.toggle--checkbox:after,
.toggle--feature,
.toggle--feature:before,
.toggle--feature:after {
  transition: all 250ms ease-in;
}
.toggle--btn:before, .toggle--btn:after,
.toggle--checkbox:before,
.toggle--checkbox:after,
.toggle--feature:before,
.toggle--feature:after {
  content: '';
  display: block;
}


.toggle--daynight .toggle--btn,
.toggle--like .toggle--btn {
  position: relative;
  height: 70px;
  width: 125px;
  border-radius: 70px;
}
.toggle--daynight .toggle--btn:before,
.toggle--like .toggle--btn:before {
  position: absolute;
  top: 2px;
  left: 4px;
  width: 56px;
  height: 56px;
  border-radius: 50%;
}

.toggle--daynight .toggle--btn {
  border: 5px solid #1c1c1c;
  background-color: #3c4145;
}
.toggle--daynight .toggle--btn:before {
  background-color: #fff;
  border: 5px solid #e3e3c7;
}
.toggle--daynight .toggle--btn:after {
  position: absolute;
  top: 62%;
  left: 39px;
  z-index: 10;
  width: 11.2px;
  height: 11.2px;
  opacity: 0;
  background-color: #fff;
  border-radius: 50%;
  box-shadow: #fff 0 0, #fff 3px 0, #fff 6px 0, #fff 9px 0, #fff 11px 0, #fff 14px 0, #fff 16px 0, #fff 21px -1px 0 1px, #fff 16px -7px 0 -2px, #fff 7px -7px 0 1px, #d3d3d3 0 0 0 4px, #d3d3d3 6px 0 0 4px, #d3d3d3 11px 0 0 4px, #d3d3d3 16px 0 0 4px, #d3d3d3 21px -1px 0 5px, #d3d3d3 16px -7px 0 1px, #d3d3d3 7px -7px 0 5px;
  transition: opacity 100ms ease-in;
}
@keyframes starry_star {
  50% {
    background-color: rgba(255, 255, 255, 0.1);
    box-shadow: #fff 30px -3px 0 0, #fff 12px 10px 0 -1px, rgba(255, 255, 255, 0.1) 38px 18px 0 1px, #fff 32px 34px 0 0, rgba(255, 255, 255, 0.1) 20px 24px 0 -1.5px, #fff 5px 38px 0 1px;
  }
}
@keyframes bounceIn {
  0% {
    opacity: 0;
    transform: scale(0.3);
  }
  50% {
    opacity: 100;
    transform: scale(1.1);
  }
  55% {
    transform: scale(1.1);
  }
  75% {
    transform: scale(0.9);
  }
  100% {
    opacity: 100;
    transform: scale(1);
  }
}
.toggle--daynight .toggle--feature {
  display: block;
  position: absolute;
  top: 9px;
  left: 52.5%;
  z-index: 20;
  width: 4px;
  height: 4px;
  border-radius: 50%;
  background-color: #fff;
  box-shadow: rgba(255, 255, 255, 0.1) 30px -3px 0 0, rgba(255, 255, 255, 0.1) 12px 10px 0 -1px, #fff 38px 18px 0 1px, rgba(255, 255, 255, 0.1) 32px 34px 0 0, #fff 20px 24px 0 -1.5px, rgba(255, 255, 255, 0.1) 5px 38px 0 1px;
  animation: starry_star 5s ease-in-out infinite;
}
.toggle--daynight .toggle--feature:before {
  position: absolute;
  top: -2px;
  left: -25px;
  width: 18px;
  height: 18px;
  background-color: #fff;
  border-radius: 50%;
  border: 5px solid #e3e3c7;
  box-shadow: #e3e3c7 -28px 0 0 -3px, #e3e3c7 -8px 24px 0 -2px;
  transform-origin: -6px 130%;
}
.toggle--daynight .toggle--checkbox:checked + .toggle--btn {
  background-color: #9ee3fb;
  border: 5px solid #86c3d7;
}
.toggle--daynight .toggle--checkbox:checked + .toggle--btn:before {
  left: 55px;
  background-color: #ffdf6d;
  border: 5px solid #e1c348;
}
.toggle--daynight .toggle--checkbox:checked + .toggle--btn:after {
  opacity: 100;
  animation-name: bounceIn;
  animation-duration: 0.60s;
  animation-delay: 0.10s;
  animation-fill-mode: backwards;
  animation-timing-function: ease-in-out;
}
.toggle--daynight .toggle--checkbox:checked + .toggle--btn > .toggle--feature {
  opacity: 0;
  box-shadow: rgba(255, 255, 255, 0.1) 30px -3px 0 -4px, rgba(255, 255, 255, 0.1) 12px 10px 0 -5px, #fff 38px 18px 0 -3px, rgba(255, 255, 255, 0.1) 32px 34px 0 -4px, #fff 20px 24px 0 -5.5px, rgba(255, 255, 255, 0.1) 5px 38px 0 -3px;
  animation: none;
}
.toggle--daynight .toggle--checkbox:checked + .toggle--btn > .toggle--feature:before {
  left: 25px;
  transform: rotate(70deg);
}
	</style>
</head>
<body>
	<div class="toggle toggle--daynight">
			<input type="checkbox" id="toggle--daynight" class="toggle--checkbox">
			<label class="toggle--btn" for="toggle--daynight"><span class="toggle--feature"></span></label>
	</div>
</body>
</html>
  </code>
</body>

