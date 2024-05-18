# Homework 2
- 과제일: 2024년 5월 10일
- 과제 내용: Naver 로그인 화면
***
## HTML
1. ```img``` 태그와 ```a```를 활용하여 로고 이미지를 마크업했습니다.

```html
<h1><a href="/" tabindex="-1"><img class="logo" src="./logo.svg" alt="네이버" /></a></h1>
```

## CSS
1. 
```css
input:focus-visible + label {
        outline: 2px solid var(--focus_color);
        border-radius: 0.25em;
      }

      input:checked + label {
        &::before {
          content: "";
        }

        &::after {
          content: "ON";
          color: #03cf5d;
        }
      }
```

***
## 리뷰
토요일에 약속이 있어서 시간에 쫓기면서 하다보니 완벽하게 하지 못 해 아쉬운 점이 남는다.
