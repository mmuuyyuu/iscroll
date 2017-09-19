IScoroll实例：下拉刷新，滚动翻页。
iscroll.js 版本4

注意：1每次加载数据必须执行1次refresh()方法，刷新一下界面。

      2.注册事件方法：
	  2.1 iscroll.js 140行 注册事件方法，例如  onScrollLimit:null,
	  2.2             497  拖动的时候    例如  if( newY < (that.maxScrollY + 250)){that.options.onScrollLimit.call(that, e);}else{that.options.onScrollElseLimit.call(that, e);};

	  2.3             780  -- 初始化do   例如  if(step.y < that.maxScrollY){that.options.onScrollLimit.call(that);}      