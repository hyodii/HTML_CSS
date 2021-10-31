# HTML & CSS 공부
## ▪ position & flexbox
**flexbox연습하는 웹사이트🐸**: [https://flexboxfroggy.com/#ko](https://flexboxfroggy.com/#ko)

### **Position속성에 값들🎈**

1. static : 웹사이트의 기본 속성값

2. relative: HTML태그가 있는 위치에서 left right top bottom값을 통해 움직임

3. absolute: 부모영역에서  left right top bottom 을 이용해 주어진 위치로 움직임

4. fixed : absolute와 비슷하지만 스크롤로 내려도 그 위치에 고정 (top 버튼같은 거에 사용)

5. Sticky : relative와 비슷하지만 스크롤로 내리면 fixed처럼 그 위치에 고정

### **flexbox 의 특징!🎊**

1. display: flex는 모든 요소를 가로로 둔다

2. display: flex는 부모한테 적용을 하고 자손을 건트롤 한다.

3. justify-content :가로로 요소들을 움직인다 

(flex-start : 왼쪽에 붙게

, center :  가운데 붙게

, flex-end : 왼쪽에 붙게

, space-between : 간격을 일정하게 띄우기

, space-around 너무끝말고 일정하게 띄우기

 등의 값이 있음)

4. align-items: 세로로 요소들을 움직인다

5. flex-direction: column 가로로 정렬된 요소를 세로로 바꾸고 justify-content는 세로로 align-items는 가로방향으로 바뀐다

++ flex-direction

- **`row`**: 요소들을 텍스트의 방향과 동일하게 정렬합니다.
- **`row-reverse`**: 요소들을 텍스트의 반대 방향으로 정렬합니다.
- **`column`**: 요소들을 위에서 아래로 정렬합니다.
- **`column-reverse`**: 요소들을 아래에서 위로 정렬합니다.

++  **`align-self`**  속성은 개별적인 콘텐츠 아이템의 정렬 상태를 설정합니다.

++ 

때때로 컨테이너의 row나 column의 순서를 역으로 바꾸는 것만으로는 충분하지 않습니다. 이러한 경우에는 **`order`** 속성을 각 요소에 적용할 수 있습니다. order의 기본 값은 0이며, 양수나 음수로 바꿀 수 있습니다.

```css
#pond {
  display: flex;
}

.yellow {
order:1
}
```

++ **`flex-wrap` :  요소들을 여러줄에 걸쳐서 정렬**

- **`nowrap`**: 모든 요소들을 한 줄에 정렬합니다.
- **`wrap`**: 요소들을 여러 줄에 걸쳐 정렬합니다.
- **`wrap-reverse`**: 요소들을 여러 줄에 걸쳐 반대로 정렬합니다.


++ **`flex-direction`** 과 **`flex-wrap`** 이 자주 같이 사용되기 때문에, **`flex-flow`** 가 이를 대신할 수 있습니다.


**flex-flow: row wrap  ←  이런식으로**

++ **`align-content`** 를 사용하여 여러 줄 사이의 간격을 지정할 수 있습니다. 이 속성은 다음의 값들을 인자로 받습니다:

- **`flex-start`**: 여러 줄들을 컨테이너의 꼭대기에 정렬합니다.
- **`flex-end`**: 여러 줄들을 컨테이너의 바닥에 정렬합니다.
- **`center`**: 여러 줄들을 세로선 상의 가운데에 정렬합니다.
- **`space-between`**: 여러 줄들 사이에 동일한 간격을 둡니다.
- **`space-around`**: 여러 줄들 주위에 동일한 간격을 둡니다.
- **`stretch`**: 여러 줄들을 컨테이너에 맞도록 늘립니다.
