## CSS制作毛玻璃效果

```css
.blur{
  -webkit-filter:blur(5px);
  -moz-filter:blur(5px);
  filter: url(data:image/svg+xml;base64,77u/PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxmaWx0ZXIgaWQ9ImJsdXIiPjxmZUdhdXNzaWFuQmx1ciBzdGREZXZpYXRpb249IjI1IiAvPjwvZmlsdGVyPjwvc3ZnPg==#blur);
  filter: blur(5px);
  filter:progid:DXImageTransform.Microsoft.Blur(PixelRadius='5');
  transition: 1s filter linear;
}
```

## 让CSS所有动画hover带有过渡效果

```
transition: all 2s;
-moz-transition: all 2s; /* Firefox 4 */
-webkit-transition: all 2s; /* Safari 和 Chrome */
```

## CSS实现单行、多行文本溢出显示省略号（…）

**单行实现**

```
overflow: hidden;
text-overflow:ellipsis;
white-space: nowrap;
```

**多行实现**

```
display: -webkit-box;
-webkit-box-orient: vertical;
-webkit-line-clamp: 3;
overflow: hidden;
```