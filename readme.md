# Figma-CSS-Skins





这是一些针对 Figma.com 和 FigmaEX 插件的 CSS 样式，能够让你自定义它们的外观

## 使用
 - [FigmaEX](https://moonvy.com/figmaEX/) v1.2.4 以上版本的设置页中 "CSS 皮肤" 功能，无论是浏览器中的 Figma 还是客户端 Figma 都可以使用。
   <img width="400px" src="https://user-images.githubusercontent.com/82231420/126589576-db664b22-7770-4f2b-992a-f686cda2dc32.png">
 - Chrome 浏览器插件 [Stylish]( https://userstyles.org/)，一个通用的网站自定义样式工具。




## FigmaEX 的定制


### 工具条位置
 
 
#### 工具条位置与圆角
<img width="300px" src="https://user-images.githubusercontent.com/82231420/126590040-e4e22fd5-22fe-453b-ab81-36959ec50623.png">
 
```css
/* 工具条位置与圆角 */
body .FigmaExApp .ExBar {
    border-radius: 2px;
    right: 242px;
    top: 51px;
}
```
 
#### 工具条放到左侧
<img width="300px" src="https://user-images.githubusercontent.com/82231420/126589326-27e21bc5-5220-45cd-858d-3babe43d4119.png">

```css
/* 工具条放到左侧 */
body .FigmaExApp .ExBar {
    right: auto;
    top: 71px;
    left: 261px;
}
```

#### 黑色外观
<img width="300px" src="https://user-images.githubusercontent.com/82231420/126614311-ebc69785-c5ca-4be0-9012-668c08475604.png">

```css
/* 黑色外观 */
body .FigmaExApp .ActionItem {
    background: #2c2c2c;
}

body .FigmaExApp .ExBar .header {
    background: #2c2c2c;
}

body .FigmaExApp .ExBar .header .logo-but {
    opacity: 0;
}

body .FigmaExApp .ExBar .header .logo-but.color {
    opacity: 0.8;
}

body .FigmaExApp .ExBar .header .setting-but,
.FigmaExApp .ExBar .header .clear-but {
    filter: invert(1);
}

body .FigmaExApp .ExBar .reseize-hand {
    background: #2c2c2c;
}

body .FigmaExApp .ExBar {
    background: #252525;
}

body .figmaex-localfont-but {
    filter: invert(1);
}
body .FigmaExApp .ActionItem .action-info {
    color: #cbd0d5;
}

body .FigmaExApp .ExBar .action-list::-webkit-scrollbar-thumb {
    border: 2px solid #252525;
}

body .FigmaExApp .ActionItem .action-info .note-name {
    color: #6e7380;
}

body .FigmaExApp .ActionItem:hover {
    background: #1d1d1d;
}
```



## Figma 的定制

除了可以改 FigmaEX 的外观，也可以改 Figma 的外观，只是 Figma 的 class 不是很适合覆盖

#### 黑暗模式

<img width="300px" src="https://user-images.githubusercontent.com/82231420/126612908-dcf7a4e7-211c-46b4-8da9-accde9c3495d.png">
 


[dark](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figma-skins/dark-1.min.css)

 
