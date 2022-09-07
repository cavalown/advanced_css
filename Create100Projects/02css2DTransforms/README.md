## Transform 
[MDN參考](https://developer.mozilla.org/zh-TW/docs/Web/CSS/transform)
修改 CSS 可視化格式模型（visual formatting model）的空間維度，具有三維的概念。


#### translate
平移。
```css
# 水平移動，正值向右。
transform: translateX(10px);
# 重職移動，正值向下。
transform: translateY(-20px);
# 移動(x, -y)
transform: translate(50px, 20px);
```

#### scale
改變比例。
```css
# 水平變形
transform: scaleX(1.5);
# 垂直變形
transform: scaleY(0.5);
# 水平垂直同時變形，根據(x, y)
transform: scale(0.5, 2);
```

#### rotate
旋轉。
```css
# 順時針旋轉
transform: rotate(20deg);
# 逆時針旋轉
transform: rotate(-60deg);
# 順時針旋轉一圈
transform: rotate(1turn);
# 逆時針旋轉兩圈
transform: rotate(-2turn);

# 梯度: 400梯度 gradient是360度
transform: rotate(200grad);
```

#### skew
二維平面的傾斜轉換。
```css
# 延X軸傾斜
transform: skewX(-30deg);
# 延Y軸傾斜
transform: skewY(20deg);
# 同時延(x, y)軸兩個向量傾斜
transform: skew(20deg, 40deg);
```

#### transform origin
變化原點，變化開始的起始點。
[參考Mdn關於transform-origin](https://developer.mozilla.org/zh-TW/docs/Web/CSS/transform-origin)
```css
# 起點在top的中心
transform-origin: top;
# 起點在bottom的中心
transform-origin: bottom;
# 起點在right的中心
transform-origin: right;
# 起點在left的中心
transform-origin: left;
# 起點在top的最right
transform-origin: top right;
# 起點在top的最left
transform-origin: top left;
# 以此類推......
        
# 以左上為起點，延伸的(x, y)位置，可以用各種長度的單位。
transform-origin: 10% 30%;
```



