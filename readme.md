# Figma-CSS-Skins





这是一些针对 Figma.com 和 FigmaEX 插件的 CSS 样式，能够让你自定义它们的外观

## 使用
 - [FigmaEX](https://moonvy.com/figmaEX/) v1.2.4 以上版本的设置页中 "CSS 皮肤" 功能，无论是浏览器中的 Figma 还是客户端 Figma 都可以使用。
   <img width="400px" src="https://user-images.githubusercontent.com/82231420/126589576-db664b22-7770-4f2b-992a-f686cda2dc32.png">
 - Chrome 浏览器插件 [Stylish]( https://userstyles.org/)，一个通用的网站自定义样式工具。




## FigmaEX 的定制


### 工具条位置
 
 
#### 工具条位置与圆角
<img width="200px" src="https://user-images.githubusercontent.com/82231420/126590040-e4e22fd5-22fe-453b-ab81-36959ec50623.png">
 
```css
/* 工具条位置与圆角 */
body .FigmaExApp .ExBar {
    border-radius: 2px;
    right: 242px;
    top: 51px;
}
```
 
#### 工具条放到左侧
<img width="200px" src="https://user-images.githubusercontent.com/82231420/126589326-27e21bc5-5220-45cd-858d-3babe43d4119.png">

```css
/* 工具条放到左侧 */
body .FigmaExApp .ExBar {
    right: auto;
    top: 71px;
    left: 261px;
}
```

## Figma 的定制

除了可以改 FigmaEX 的外观，也可以改 Figma 的外观，只是 Figma 的 class 不是很适合覆盖

#### 黑暗模式



[dark](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figma-skins/dark-1.css)

 
