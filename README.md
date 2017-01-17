# Tetris
网页版的俄罗斯方块小游戏

设计思路：
1.用一个div作为游戏主界面，height：400，width：200，position：relative。
2.主界面div内放置200个无边框，透明的span，height：20，width：20，float：left，display：inline-block；
  定义一个spansObj对象存放每个坐标点上的span。
3.图形用一个div表示，height和width根据图形的不同而设定，里面放置span，height：20，width：20，float：left，display：inline-block；
  定义一个posObj对象存放每个span相对于图形div的坐标和值。
4.用一个定时器控制图形div的top和left。
5.当图形div达到目的坐标后，移除该div，将主界面中对应位置的span设置样式，将其显示出来。
