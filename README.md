## 栅格系统简介
- 针对不同浏览器窗口尺寸进行响应式设计，栅格系统会根据尺寸变化，自动显示适当的元素大小比例，有利于在各种窗口条件下浏览页面。
## 实现原理
- 通过CSS的媒体查询获取当前浏览器窗口尺寸，为各元素预设相应条件下合适的相对比例（及位置），从而实现自动响应。
## 使用方法
- 每个元素预设可以有4级宽度的变化，分别对应xs sm lg xl后缀的1 2 3 4，通过在 `grid-system.css` 中添加级别，可以增加宽度变化的范围和细腻程度。
- 窗口宽度尺寸有4级阈值响应，分别对应xs(>1200px) ms(>992px) lg(>768px) xl(<768px)，通过在 `grid-system.css` 中添加阈值，亦能增加窗口响应密度和范围。
- 使用时，修改 `demo.html` 中元素的 `class` 值为对应窗口尺寸下的期望值即可。
- 举例：如 `sm-2` 指在窗口尺寸为sm时显示对应元素为第2级大小， `xl-4` 指在窗口尺寸为xl时显示对应元素为第4级大小。