## flex-grow

작성자 : 김동일

작성일 : 2015-10-30

css 레퍼런스 설명:
 - flex-grow : div 영역 내 flex item 들의 비율로 늘려 크기를 설정한다.

 - syntax :
```sh
flex-grow: number|initial|inherit;
```

number : flex item 별로 비율을 설정한다.(기본값 : 0)

initial:기본 값으로 set되어 있는 값을 불러온다.

inherit:부모 element에 설정되어 있는 값을 상속 받는다.

sample code :
```html
<!DOCTYPE html>
<html>
<head>
<style>
#main {
    width: 350px;
    height: 100px;
    border: 1px solid #c3c3c3;
    display: -webkit-flex; /* Safari */
    display: flex;
}

/* Safari 6.1+ */
#main div:nth-of-type(1) {-webkit-flex-grow: 1;}
#main div:nth-of-type(2) {-webkit-flex-grow: 3;}
#main div:nth-of-type(3) {-webkit-flex-grow: 1;}
#main div:nth-of-type(4) {-webkit-flex-grow: 1;}
#main div:nth-of-type(5) {-webkit-flex-grow: 1;}

/* Standard syntax */
#main div:nth-of-type(1) {flex-grow: 1;}
#main div:nth-of-type(2) {flex-grow: 3;}
#main div:nth-of-type(3) {flex-grow: 10;}
#main div:nth-of-type(4) {flex-grow: 1;}
#main div:nth-of-type(5) {flex-grow: 1;}
</style>
</head>
<body>

<div id="main">
  <div style="background-color:coral;"></div>
  <div style="background-color:lightblue;"></div>
  <div style="background-color:khaki;"></div>
  <div style="background-color:pink;"></div>
  <div style="background-color:lightgrey;"></div>
</div>

<p><b>Note:</b> Internet Explorer 10 and earlier versions do not support the flex-grow property.</p>

<p><b>Note:</b> Safari 6.1 (and newer) supports an alternative, the -webkit-flex-grow property.</p>

</body>
</html>
```

결과

![flex-grow](../images/flex-grow.jpg)



-----

* [CSS3 README](../README.md)

* [flex](flex.md)
* [flex-basis](flex-basis.md)
* [flex-direction](flex-direction.md)
* [flex-flow](flex-flow.md)
* [flex-grow](flex-grow.md)
* [flex-shrink](flex-shrink.md)
* [flex-wrap](flex-wrap.md)
