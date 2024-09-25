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
 
- [**复制风格**](https://github.com/liteyais/FigmaEX-CSS-Skin)


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
<img width="912" alt="im321" src="https://github.com/user-attachments/assets/e54bd27a-9a1e-472b-9c94-def387598510">


  
解决方案有两个  
方案一：[**Alban-白**](https://gist.githubusercontent.com/shangrenxi/1f4ec563435cba83a00bfcfdb444f551/raw/figmaEX-Enhance.css)  
方案二：[**@Ma200line**](https://gist.githubusercontent.com/tr0j4ndev/9d6f1f7ac541910b861665944899e3b9/raw/figmaui3&figmaex.txt)  
[两个方案的区别可以前往打开 Figma 文件查看具体对比](https://www.figma.com/design/zR01HW7LaUE43OrSu3jhdY/Figma-%E6%9C%80%E8%BF%91%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98?node-id=8155-12&t=rgrOuotWK54hFw98-1)  

       
 
 
