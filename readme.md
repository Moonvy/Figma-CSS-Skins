# Figma-CSS-Skins



这是一些针对 Figma.com 和 FigmaEX 插件的 CSS 样式，能够让你自定义它们的外观

## 使用
 - [FigmaEX](https://moonvy.com/figmaEX/) v1.2.4 以上版本的设置页中 "CSS 皮肤" 功能，无论是浏览器中的 Figma 还是客户端 Figma 都可以使用。
   <img width="400px" src="https://user-images.githubusercontent.com/82231420/126589576-db664b22-7770-4f2b-992a-f686cda2dc32.png">
 - Chrome 浏览器插件 [Stylish]( https://userstyles.org/)，一个通用的网站自定义样式工具。


## 支持定制的范围
- [插件工具条的外观](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/readme.md#%E6%8F%92%E4%BB%B6%E5%B7%A5%E5%85%B7%E6%9D%A1%E7%9A%84%E5%A4%96%E8%A7%82%E5%AE%9A%E5%88%B6)
- [Figma UI3 选中图层上下文面板的外观](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/readme.md#figma-ui3-%E9%80%89%E4%B8%AD%E5%9B%BE%E5%B1%82%E4%B8%8A%E4%B8%8B%E6%96%87%E9%9D%A2%E6%9D%BF%E7%9A%84%E5%A4%96%E8%A7%82)
- [Figam UI3 左右面板的圆角和间距外观（梦回UI2）](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/readme.md#figam-ui3-%E5%B7%A6%E5%8F%B3%E9%9D%A2%E6%9D%BF%E7%9A%84%E5%9C%86%E8%A7%92%E5%92%8C%E9%97%B4%E8%B7%9D%E5%A4%96%E8%A7%82%E6%A2%A6%E5%9B%9Eui2)

## 插件工具条的外观定制

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

 ## 其他工具条的配色主题
 
 #### 茶茶头像卡通风格
<img width="300px" src="https://user-images.githubusercontent.com/82380792/223678797-45e77d42-1a79-4b04-b2d3-b4e3542af31f.gif">

感谢 [**liteyais**](https://github.com/liteyais) 提供的配色和非常好玩的交互动画
 
- [**头像版**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/EX%E6%8F%92%E4%BB%B6%E8%8C%B6%E8%8C%B6%E6%A9%99-%E5%A4%B4%E5%83%8F%E7%89%88-%E4%B8%8D%E5%B8%A6%E8%84%9A.css)  
- [**全身版v2.3**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/%E8%8C%B6%E8%8C%B6%E7%9A%AE%E8%82%A4-%E5%85%A8%E8%BA%AB%E7%89%88-%E6%B5%85%E8%89%B2%E6%B7%B1%E8%89%B2%E9%80%9A%E7%94%A8%E7%89%88v2.3.css)
- [**作者设计的其他风格以及更新**](https://github.com/liteyais/FigmaEX-CSS-Skin)


#### 粉萌萌模式

 <img width="300px" src="https://user-images.githubusercontent.com/82380792/126638949-2c83310c-b89e-42f2-b65d-1817373cfcfb.png">

[**Pink CSS**](https://github.com/Moonvy/Figma-CSS-Skins/blob/master/figmex-skins/%E7%B2%89%E8%90%8C%E8%90%8C.css)

---  

## Figma UI3 选中图层上下文面板的外观

#### 白色外观
<img width="500" alt="im321" src="https://github.com/user-attachments/assets/1aaa050c-87f4-4ad0-a8cd-df6e13f384fc">

 
 
感谢 [**Alban-白**](https://github.com/shangrenxi) 提供的配色和非常详细的代码注释

```css
.positioned_design_toolbelt--root--INYO4 {
/*    top: 12px !important;*/
    left: -16%;
}

/*EX上下文增强工具*/
.ExContextPad {
    background: var(--color-bg);
    left: calc(42% + 220px);
    bottom: 12px;
    height: 40px;
    border: none;
    border-radius: var(--radius-large);
}


/*选项菜单浮层*/
.AbMenuRoot .oMenuList.shadow {
    background:var(--color-bg);
    color: var(--color-text, #333);
    border-radius: var(--radius-medium);
    box-shadow: var(--elevation-200-canvas);
}


/*上下文图标*/
.ExContextPad button img {
    filter: invert(1);
}

[data-preferred-theme=dark] {
  .ExContextPad button img {
      filter: unset;
  }
}

/*图标hover*/
.ExContextPad button img:hover {
    background: rgb(255 255 255 / 4%);
    border-radius: var(--radius-medium);
}

/*图标间距*/
.ExContextPad hr {
/*    display: none;*/
    background: var(--color-border);
}
```

## Figam UI3 左右面板的圆角和间距外观（梦回UI2）
 #### 去掉左右面板的圆角以及边距,让中间的操作区域更大  
<img width="400px" src="https://private-user-images.githubusercontent.com/82380792/356159029-271c8586-8d74-4cb1-b396-5face781a1ed.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjMxMDg3NjcsIm5iZiI6MTcyMzEwODQ2NywicGF0aCI6Ii84MjM4MDc5Mi8zNTYxNTkwMjktMjcxYzg1ODYtOGQ3NC00Y2IxLWIzOTYtNWZhY2U3ODFhMWVkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA4MDglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwODA4VDA5MTQyN1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTM4MTAyYTRlZDMxNjY1YTg2MDg4ZmQzYzg4NzliZDU3M2YyMGIwYTg4MTliZDkwZmY2YWE3Y2Y5MThlMTNhYTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.TCqXLtvz7evKE6W2fUXVqTi6j97l_dvssnEblxsTM1I">  
  
解决方案有两个  
方案一：[**Alban-白**](https://gist.githubusercontent.com/shangrenxi/1f4ec563435cba83a00bfcfdb444f551/raw/figmaEX-Enhance.css)  
方案二：[**@Ma200line**](https://gist.githubusercontent.com/tr0j4ndev/9d6f1f7ac541910b861665944899e3b9/raw/gistfile1.txt)  
[两个方案的区别可以前往打开 Figma 文件查看具体对比](https://www.figma.com/design/zR01HW7LaUE43OrSu3jhdY/Figma-%E6%9C%80%E8%BF%91%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98?node-id=8155-12&t=rgrOuotWK54hFw98-1)  

       
 
 
