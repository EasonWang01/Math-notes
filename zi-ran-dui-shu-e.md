# 自然對數e

[https://zh.wikipedia.org/wiki/E\_(数学常数\\](https://zh.wikipedia.org/wiki/E\_\(%E6%95%B0%E5%AD%A6%E5%B8%B8%E6%95%B0/)

往下拉到定義部分

## 1.

```
定義 e 爲下列極限值：
```

![](<.gitbook/assets/螢幕快照 2018-02-16 上午10.13.42.png>)

可用程式計算

> n趨近極大值

```javascript
function a (n){return (1+1/n) ** n }

// a(9000000000)
// 2.718282053219686
```

以及

![](<.gitbook/assets/螢幕快照 2018-02-16 上午10.14.16.png>)

> n趨近極小值

```javascript
function b (n){return (1+n) ** (1/n) }

// b(0.000000000001)
// 2.7185234960372378
```

> 但javascript有最大限制
>
> [http://stackoverflow.com/questions/43729790/natural-logarithm-e-1](http://stackoverflow.com/questions/43729790/natural-logarithm-e-1)

## 2.

```
定義 e 爲下列無窮級數之和：
```

可用程式計算

```
//fact用來計算階層的倒數
function fact(x) {
   if(x==0) {
      return 1;
   }
   return 1 / x * fact(x-1) ;
}


function c(n) {
  var total = fact(n);
  for(i = 1; i <= n; i++ ){
    total += fact(n - i)
  }
 return total;
}

//c(345)
```

\>以上兩者給n到一數以上時都會為2.7.......

## 當![{\displaystyle x=e}](https://wikimedia.org/api/rest\_v1/media/math/render/svg/8ba47ab1931fc4886c5da08831962cc141d20655)時函數![f(x) = \sqrt\[x\]{x}](https://wikimedia.org/api/rest\_v1/media/math/render/svg/e15600c8e263f973cca6db5347531ea5a6846aa8)有最大值

```javascript
Math.newsqrt = function(a, b) {
  if(b > 0) {
    a = Math.sqrt(a);
    return Math.newsqrt(a, b - 1);
  } else {
    return a
  }
}

Math.newsqrt(Math.exp(1), Math.exp(1))
```

[http://blog.udn.com/cchahacaptain/4565752](http://blog.udn.com/cchahacaptain/4565752)
