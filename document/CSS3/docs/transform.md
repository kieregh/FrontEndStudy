# transform

작성자 : 장현웅

작성일 : 2015-11-10

css 레퍼런스 설명: 시각적 서식 모델(visual formatting model)의 좌표 공간을 변형시킬 수 있다. 해당 속성에 지정된 값에 따라 엘리먼트(element)에 이동(translate), 회전(rotate), 크기변경(scale), 기울임(skew)등의 효과를 줄 수 있다.

syntax:
```
transform : transform-function | none;
```

2D 속성
none : 변형 속성을 적용하지 않음

translate(x,y):	요소의 위치를 옮기는 속성

scale(x,y) : 요소의 크기를 비율에 맞춰 확대/축소하는 속성

rotate(angle) : 요소를 지정된 각도 만큼 회전시키는 속성

skew(x-angle, y-angle) : 요소를 지정된 각도만큼 모양을 비스듬히 변형시키는 속성

matrix(n,n,n,n,n,n)	: translate, scale, rotate, skew 각 속성을 한꺼번에 적용할 수 있는 매트릭스 함수


sample code :
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="EUC-KR">
<title>Insert title here</title>
<style>
div {
    width: 200px;
    height: 100px;
    margin-bottom: 50px;
}
.none {
	transform: none;
    background-color: yellow;
}
.translate {
	transform: translate(12px, 20%);
    background-color: red;
}
.scale {
	transform: scale(0.5, 1.5);
    background-color: green;
}
.rotate {
	transform: rotate(0.2turn);
    background-color: blue;
}
.skew {
	transform: skew(-35deg,-200deg);
    background-color: grey;
}
</style>
</head>
<body>

<div class="none">none</div>
<div class="translate">translate</div>
<div class="scale">scale</div>
<div class="rotate">rotate</div>
<div class="skew">skew</div>

</body>
</html>
```

## [실행결과 보기](http://codepen.io/jhw811/pen/meaLgd)



3D 속성

translate3d(x,y,z) : 요소의 위치를 옮기는 속성

translateX(x) : 요소의 x 좌표 위치를 옮기는 속성

translateY(y) : 요소의 y 좌표 위치를 옮기는 속성

translateZ(z) : 요소의 z 좌표 위치를 옮기는 속성

scale3d(x,y,z) : 요소의 크기를 비율에 맞춰 확대/축소하는 속성

scaleX(x) : 요소의 x축 크기를 비율에 맞춰 확대/축소하는 속성

scaleY(y) : 요소의 y축 크기를 비율에 맞춰 확대/축소하는 속성

scaleZ(z) : 요소의 z축 크기를 비율에 맞춰 확대/축소하는 속성

rotate3d(x,y,z,angle) : 요소를 지정된 각도 만큼 회전시키는 속성

rotateX(angle) : 요소를 지정된 각도 만큼 x축을 회전시키는 속성

rotateY(angle) : 요소를 지정된 각도 만큼 y축을 회전시키는 속성

rotateZ(angle) : 요소를 지정된 각도 만큼 z축을 회전시키는 속성

skewX(angle) : 요소를 지정된 각도만큼 x축 모양을 비스듬히 변형시키는 속성

skewY(angle) : 요소를 지정된 각도만큼 y축 모양을 비스듬히 변형시키는 속성

skewZ(angle) : 요소를 지정된 각도만큼 z축 모양을 비스듬히 변형시키는 속성

perspective(n) : 지정된 픽셀만큼 더 멀리서 보는 효과를 낸다

matrix3d(n,n,n,n,n,n,n,n,n,n,n,n,n,n,n,n) : translate, scale, rotate, skew 각 속성을 한꺼번에 적용할 수 있는 매트릭스 함수




sample code :
```html

<!DOCTYPE html>
<html>
<head>
<meta charset="EUC-KR">
<title>Insert title here</title>
<style>
div {
    width: 200px;
    height: 100px;
    margin-bottom: 50px;
}
.none {
	transform: none;
    background-color: yellow;
}
.translate3d {
	transform: translate3d(20px, 30px, 40px);
    background-color: red;
}
.scale3d {
	transform: scale3d(0.5, 1.5,1.5);
    background-color: green;
}
.rotate3d {
	transform: rotate3d(1, 0, 1, 80deg);
    background-color: blue;
}
.skewX {
	transform: skewX(30deg);
    background-color: grey;
}
.skewY {
	transform: skewY(30deg);
    background-color: cyan;
}

</style>
</head>
<body>
<div class="none">none</div>
<div class="translate3d">translate3d</div>
<div class="scale3d">scale3d</div>
<div class="rotate3d">rotate3d</div>
<div class="skewX">skewX</div>
<div class="skewY">skewY</div>
</body>
</html>
```


## [실행결과 보기](http://codepen.io/jhw811/pen/PPXeLP)



-----

* [CSS3 README](../README.md)

* [transform](transform.md)
* [transform-origin](transform-origin.md)
* [transform-style](transform-style.md)
