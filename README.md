# Css Practice

## 상대 단위 종류

### Em

```
요소의 font-size으로 기준으로 px 계산
```

```
아래와 같이 font-size를 20px 잡을 경우 width은 20px * 10 이므로 width가  200px 으로 설정
```

```css
.em_container {
  font-size: 20px;
  width: 10em; /* 20 * 10 */
  height: 30px;
  background-color: antiquewhite;
  margin: 0 auto;
  margin-top: 83px;
}
```

### Rem

```
루트요소의 font-size으로 기준으로 px 계산
```

```
아래와 같이 루트 font-size를 16px 잡을 경우 width은 16px * 10 이므로 width가  160px 으로 설정
```

```css
html {
  font-size: 16px;
}
.rem_container {
  width: 10rem; /* 16 * 10 = 160 */
  height: 30px;
  background-color: ghostwhite;
  margin: 0 auto;
}
```

### vw

```
현재 너비의 비율로 계산
현재 너비 1200px 이면
1vw = 1200 / 100 = 12px
width : 30vw 으로 설정하면
12px * 30 = 3600px
```

```css
.vw_container {
  width: 30vw; /* 1200px / 100 = 12 , 1vw = 12px , 12 * 30 = 360px */
  height: 30px;
  background-color: blue;
  margin: 0 auto;
}
```

### vh
