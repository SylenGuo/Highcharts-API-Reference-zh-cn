Highcharts.setOptions
===================================
   ### global

	global选项和lang选项一样并不一定适合每一张图表, 必须使用 Highcharts.setOptions 函数才能使其生效。
	例如：
	````c
	Highcharts.setOptions({
		global: {
			useUTC: false
		}
	});
	````

  	**VMLRadialGradientURL**: String     所需版本 2.3.0+

	VML浏览器绘制图形渐变所需图片路径 (version:版本号)
	默认URL路径： http://code.highcharts.com/{version}/gfx/vml-radial-gradient.png

	**canvasToolsURL**: String

	此选项延迟加载文件用于支持Android 2.x设备，由于此设备并不支持SVG，所以进行额外包含[canvg](<http://code.google.com/p/canvg/>)。此功能依赖rbcolor和Highcharts CanVG渲染器。
	
	为了第三方安全问题，请使用Hightcharts官网的canvas-tools.js文件.
	地址为：http://code.highcharts.com/{version}/modules/canvas-tools.js

	**useUTC**: Boolean

	是否使用UTC标准时间，例如在坐标轴上，刻度线分布以及 Highcharts.dateFormat 函数格式化。使用UTC的好处是不管浏览用户在什么时区，都会看到相同的结果。
	当操作实时数据或者当前为夏令时，时间将被转换。 **默认值：true**
	
	试一试:<br /> 
		* [默认值为true](<http://jsfiddle.net/gh/get/jquery/1.7.2/highslide-software/highcharts.com/tree/master/samples/highcharts/global/useutc-true/>) - 起始点为 00:00 UTC，在坐标轴(axis)和消息提示(tooltip)时将会显示 00：00<br />
		* 当为false时  - 起始点为 00:00 UTC，在坐标轴(axis)和消息提示(tooltip)时将会显示浏览者本地机器时间

   ### lang
    翻译中...