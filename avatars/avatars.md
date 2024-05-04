# Homework 1
- 과제일: 2024년 5월 3일
- 과제 내용: Avatars - float, flex를 활용하여 레이아웃 완성하기
***
## HTML
1. ```img``` 태그를 활용하여 콘텐츠 이미지로 마크업했습니다.

```html
<img class="images" src="../images/faces/face1.jpg" alt="여성 얼굴1" />
```
2. ```div``` 태그를 활용하여 온라인/오프라인을 구분하는 아이콘을 만들었으며 aria-label 속성도 부여하여 접근성을 향상해보았습니다.
```html
<div class="offline" aria-label="오프라인"></div>
<div class="online" aria-label="온라인"></div>
```
3. 이후 person 클래스와 women, men 클래스 태그를 그룹화하였습니다.
```html
<div class="women">
  <div class="person">
    ...
  </div>
</div>
<div class="men">
  <div class="person">
    ...
  </div>
</div>
```

## CSS
1. 이미지와 온라인/오프라인 상태에 원형인 부분을 ```border-radius``` 속성을 활용하여 원형을 구현하였습니다.
```css
border-radius: 100%;
```
2. ```float``` 속성을 person 클래스에 적용하였습니다.
```css
.person {
  float: left;
}
```
3. 온라인/오프라인을 나타내는 부분은 ```position```을 활용하여 각 사진을 기준으로 배치하였습니다.
```css
.online {
  background-color: #4CFE88;
  border-radius: 100%;
  border: 2px solid #FFFFFF;
  width: 20px;
  height: 20px;
  position: absolute;
  top: 55px;
  left: 55px;
}

.offline {
  background-color: #DBDBDB;
  border-radius: 100%;
  border: 2px solid #FFFFFF;
  width: 20px;
  height: 20px;
  position: absolute;
  top: 55px;
  left: 55px;
}
```
4. ```display: flex```을 사용할 수 있는 브라우저에서는 ```flex```을 사용하여 레이아웃을 구성하였습니다.
```css
@supports (display: flex) {
  body {
    display: flex;
    flex-flow: column nowrap;
  }

  .women {
    order: 2;
  }

  .men {
    order: 1;
  }
}
```
***
## 리뷰
과제의 디자인 시안을 봤을 떄에는 쉬워보였지만 막상 float을 사용하여 직접 해보니 생각대로 되지 않아 의외로 시간이 오래 걸렸다. 하지만 live server을 활용하여 바로 구현 가능하여 너무 재미있게 했던 것 같다. float 부분에서 시간이 오래걸려 해당 과제 이후 복습하는 시간을 가져야할 것 같다.
