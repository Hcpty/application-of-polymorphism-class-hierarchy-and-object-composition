# Factory

需求：用戶只需要修改一行代碼，就能夠切換產品系列。

方案：引入一個Factory對象，由Factory對象提供一系列返回產品的操作。

案例：

```Java
WidgetFactory widgetFactory = new PMWidgetFactory();
Window window = widgetFactory.createWindow();
ScrollBar scrollBar = widgetFactory.createScrollBar();
```

用戶只需要將第一行代碼修改成`WidgetFactory widgetFactory = new MotifWidgetFactory();`，就能將控件系列從Presentation Manager切換到Motif。

Factory類中用於返回產品的操作稱爲Factory Method。
