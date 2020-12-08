# π

## π

```text
π通常被定義為圓的周長 C 與直徑 d 的比值
```

```text
約等於3.14
```

π 代表180度下的弧長，`直徑 x 3.14(π)`= 整個圓的圓周長

## 弧長 \( Radians \)

單位弧長為半圓的弧長除以 `3.14 (π)` ，所以180度為3.14個單位弧長

[https://www.google.com.tw/search?q=radians&rlz=1C1CHBF\_enPH768PH769&oq=radians&aqs=chrome..69i57j69i60&sourceid=chrome&ie=UTF-8](https://www.google.com.tw/search?q=radians&rlz=1C1CHBF_enPH768PH769&oq=radians&aqs=chrome..69i57j69i60&sourceid=chrome&ie=UTF-8)

```text
a unit of measurement of angles equal to about 57.3°, equivalent to the angle subtended at the centre of a circle by an arc equal in length to the radius.
```

`π x r degree = 180度` 所以`57.3 x 3.1415 = 180`

## 角度轉為弧長

以半圓來看，`單位弧長 x π`就會是一個半圓。

所以等於`單位弧長(1) x π = 180°`

這時候如果我們要算20度為多少弧長時只要先計算每一度是多少弧長，然後再乘以20即可。

`單位弧長(1) x π / 180 = 1°`

所以

```javascript
function toRadians (angle) {
  return angle * (Math.PI / 180);
}
```

所以要算sin\(90°\)則為 :

```text
Math.sin(90 * Math.PI / 180)
```

## 圓面積公式推導

圓面積 = pi \* \(r \*\*2\) = \(\(1/2\) \* r\) \* 圓周長 

> r = 半徑;  圓周長 = 2 \* r \* pi
>
> 可用微積分想像將圓切成很多個三角形然後面積加總

[https://www.youtube.com/watch?v=RCJmYfRoCwA](https://www.youtube.com/watch?v=RCJmYfRoCwA)

