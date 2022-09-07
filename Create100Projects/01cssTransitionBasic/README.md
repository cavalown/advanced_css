# CSS Transition 轉場

## Transition
#### transition-property
指定要改變的property，若要指定多個，可用空格隔開，若要指定全部可用all代替。
```css
transition-property: color;
transition-property: color backrground-color;
transition-property: all;
```

#### transition-duration
轉場變化總時間。
```css
transition-duration: 2s;
transition-duration: 2000ms;
```

#### transition-timing-function
轉場的漸變函數，貝茲曲線。有四個已經定義好的韓式：
- ease = cubic-bezier(0.25, 0.1, 0.25, 1.0)
- linear = cubic-bezier(0.0, 0.0, 1.0, 1.0)
- ease-in = cubic-bezier(0.42, 0, 1.0, 1.0)
- ease-out = cubic-bezier(0, 0, 0.58, 1.0)
- ease-in-out = cubic-bezier(0.42, 0, 0.58, 1.0)
```css
transition-timing-function: ease;
transition-timing-function: ()
```

#### transition-delay
轉場開始的時間。
```css
transition-delay: 3s;
```

#### transition
合併上述。若有多個property，用","隔開，若需要全部property，用"all"替代。
```css
transition: property transition-duration transition-timing-function transition-delay

transition: color 3s ease-in 5s
```

#### Animatable CSS properties
可以使用transition的property。
[參考連結](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties)
