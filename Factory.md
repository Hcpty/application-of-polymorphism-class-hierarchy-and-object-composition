# Factory

效果：用戶只需要修改一行代碼，就能夠切換產品系列。

方案：引入Factory，由Factory提供返回產品的操作。

案例：

```Java
WidgetFactory widgetFactory = new PMWidgetFactory();
Window window = widgetFactory.createWindow();
ScrollBar scrollBar = widgetFactory.createScrollBar();
```

用戶只需要把第一行代碼修改成`WidgetFactory widgetFactory = new MotifWidgetFactory();`，就能夠將控件系列從Presentation Manager切換到Motif。

Factory中返回產品的操作稱爲Factory Method。
