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


 
 ## 其他 FigmaEX 配色主题
 
 #### 茶茶头像卡通风格
<img width="300px" src="https://user-images.githubusercontent.com/82380792/223678797-45e77d42-1a79-4b04-b2d3-b4e3542af31f.gif">

感谢 [**liteyais**](https://github.com/liteyais) 提供的配色和非常好玩的交互动画
 
- [**头像版**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/EX%E6%8F%92%E4%BB%B6%E8%8C%B6%E8%8C%B6%E6%A9%99-%E5%A4%B4%E5%83%8F%E7%89%88-%E4%B8%8D%E5%B8%A6%E8%84%9A.css)  
- [**全身版**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/%E8%8C%B6%E8%8C%B6%E7%9A%AE%E8%82%A4-%E5%85%A8%E8%BA%AB%E7%89%88-%E6%9A%97%E9%BB%91%E6%A8%A1%E5%BC%8F.css)



#### 粉萌萌模式

 <img width="300px" src="https://user-images.githubusercontent.com/82380792/126638949-2c83310c-b89e-42f2-b65d-1817373cfcfb.png">

[**Pink CSS**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/%E7%B2%89%E8%90%8C%E8%90%8C.css)


#### DeepDark

 <img width="300px" src="https://user-images.githubusercontent.com/82380792/126982382-102a95d3-f638-44a6-9778-a7c0d77f1c08.png">

感谢 [**Alban-白**](https://github.com/shangrenxi) 提供的配色和非常详细的代码注释
[**DeepDark CSS**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/DeepDark.css)



#### 星空蓝模式

 <img width="300px" src="https://user-images.githubusercontent.com/82380792/126733168-833b5697-2c46-4284-a65f-901b3336f791.png">

感谢 Wish 提供的配色和代码注释
[**SkyBlue CSS**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/SkyBlue.css)


---  


## Figma 的定制

除了可以改 FigmaEX 的外观，也可以改 Figma 的外观，只是 Figma 的 class 不是很适合覆盖



#### 黑暗模式

<img width="300px" src="https://user-images.githubusercontent.com/82231420/126612908-dcf7a4e7-211c-46b4-8da9-accde9c3495d.png">
 


[**Dark CSS**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figma-skins/dark-1.min.css)

 
 
 #### 黑暗模式的标尺
 
 <img width="300px" src="https://user-images.githubusercontent.com/82231420/126621014-69c18066-43c5-47f0-9038-08b79bbd9cb0.png">
 
 
 如果你在黑暗模式下使用标尺，可以用这个把标尺变成黑的
 ```css
 #fullscreen-root .view.gpu-view-content::before {
    content: "";
    width: 21px;
    height: 100%;
    position: absolute;
    left: 0;
    z-index: 1;
    background: #00000082;
    backdrop-filter: invert(1) hue-rotate(212deg) brightness(2.5);
}

#fullscreen-root .view.gpu-view-content::after {
    content: "";
    width: 100%;
    height: 21px;
    position: absolute;
    left: 21px;
    top: 0;
    z-index: 1;
    background: #00000082;
    backdrop-filter: invert(1) hue-rotate(212deg) brightness(2.5);
}

 ```
 
 
