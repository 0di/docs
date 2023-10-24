# Responsive

Na potrzeby responsywności wszędzie gdzie to tylko możliwe używane sa jednostki `rem`. Wyjątkami są oczywiście miejsca gdzie wartości są bardzo małe jak np. border o grubości 1px lub inne podobne przypadki gdzie wartości na mniejszych ekranach stawałyby się ułamkami pixeli.

Na potrzeby testowania aktualnego rozmiaru ekranu można w dowolnym miejscu w kodzie (najlepiej w layout.component.html) dodać poniższy kod

```html
<div dev></div>
```

W dolnym rogu strony ukaże się aktualny 'device' i 'size' jaki interpretuje aplikacja.


## Phone

Tworząc media-query dla telefonów używamy 

```js {highlight: ['scss']}
@include phone('rozmiar'){}
//lub
@include phone(){}
```

W przypadku podania rozmiaru tworzony media query z max-width odpowiednim dla danego rozmiaru. np  

```js {highlight: ['scss']}
@include phone('md'){
    color: red;
}
//output:
@media (max-width: 540px){
    color: red;
}
```

Jeżeli nie zostanie podany rozmiar, utworzone zostanie media query obejmujące wszystkie rozmiary należące do phone. 
*W przypadku phone nie zostanie utworzone min-width: 0 bo nie ma to sensu.*

```js {highlight: ['scss']}
@include phone(){
    color: red;
}
//output:
@media (max-width: 720px){
    color: red;
}
```

|                     |   xxs   |   xs   |   sm   |   md   |   lg   |   xl   |
| ------------------- | ------- | ------ | ------ | ------ | ------ | ------ |
| Phone [0px - 720px] | do 360  | do 400 | do 480 | do 540 | do 600 | do 720 |

> Tylko `phone()` posiada rozmiar `xxs`




## Tablet

Tworząc media-query dla tabletów używamy 

```js {highlight: ['scss']}
@include tablet('rozmiar'){}
//lub
@include tablet(){}
```

W przypadku podania rozmiaru tworzony media query z max-width odpowiednim dla danego rozmiaru. np  

```js {highlight: ['scss']}
@include tablet('md'){
    color: red;
}
//output:
@media (max-width: 900px){
    color: red;
}
```

Jeżeli nie zostanie podany rozmiar, utworzone zostanie media query obejmujące wszystkie rozmiary należące do tablet. 

```js {highlight: ['scss']}
@include tablet(){
    color: red;
}
//output:
@media (max-width: 1024px) and (min-width: 721px){
    color: red;
}
```

|                         |   xs   |   sm   |   md   |   lg   |    xl   |
| ----------------------- | ------ | ------ | ------ | ------ | ------- |
| Tablet [721px - 1024px] | do 768 | do 800 | do 900 | do 960 | do 1024 |





## Desktop

Tworząc media-query dla desktopów używamy 

```js {highlight: ['scss']}
@include desktop('rozmiar'){}
//lub
@include desktop(){}
```

W przypadku podania rozmiaru tworzony media query z max-width odpowiednim dla danego rozmiaru. np  

```js {highlight: ['scss']}
@include desktop('md'){
    color: red;
}
//output:
@media (max-width: 1440px){
    color: red;
}
```

Jeżeli nie zostanie podany rozmiar, utworzone zostanie media query obejmujące wszystkie rozmiary należące do desktop. 
*W przypadku desktop nie zostanie utworzone max-width bo nie ma to sensu.*

```js {highlight: ['scss']}
@include desktop(){
    color: red;
}
//output:
@media (min-width: 1025px){
    color: red;
}
```

|                      |    xs   |    sm   |    md   |    lg   |    xl   |  two-k  |   qhd   |
| -------------------- | ------- | ------- | ------- | ------- | ------- | ------- | ------- |
| Desktop [1025px - ~] | do 1280 | do 1366 | do 1440 | do 1600 | do 1920 | do 2048 | do 2560 |

> Tylko `desktop()` posiada rozmiary `two-k` i `qhd`




## Media-range

`media-range` pozwala tworzyć media query między dowolnymi rozmiarami dowolnych urządzeń.


```js {highlight: ['scss']}
@include media-range('from-device', 'from-size' , 'to-device' , 'to-size'){}


//example:
@include media-range('phone', 'lg' , 'tablet' , 'sm'){
    color: red;
}
//output:
@media (max-width: 800px) and (min-width: 601px){
    color: red;
}
```

Możliwe jest też pozostawienie którejś pary ('from' lub 'to') pustej np.

```js {highlight: ['scss']}
@include media-range('phone', 'lg' , '' , ''){
    color: red;
}
//output:
@media (min-width: 601px){
    color: red;
}
```
