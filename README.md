# CSS

## 憎っくきIE11
Flexbox Columnを指定するとなんだかおかしいよ
```
flex-direction: column;
子要素に
flex: 0 1 auto;
width: 100%;
もしくは
flex: 0 0 auto;
}
```
<br><br>


# Other

### Chromeでaタグやcursor: pointerを設定しても指マークにならない問題。
Photoshop を立ち上げていると、ブラウザのカーソルがデフォルトから変わらないバグがあるらしいことがわかりました。なんとw


### Font Awesome 5 Freeで疑似要素(:after,:before)のcontent指定する場合
```
a::after {
  font-family: "Font Awesome 5 Free";
  content: "\f107";
  -webkit-font-smoothing: antialiased;
  display: inline-block;
  font-style: normal;
  font-variant: normal;
  text-rendering: auto;
  line-height: 1;
}
```
またBrands(ブランド系)アイコンを使う場合はfont-familyの指定が違う模様。
```
a::after {
  font-family: "Font Awesome 5 Brands";
  content: "\f099";
}
```
