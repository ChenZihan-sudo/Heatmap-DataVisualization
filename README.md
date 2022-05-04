# Heatmap-DataVisualization
简易实现热力地图数据可视化     

![image](https://user-images.githubusercontent.com/64928288/166636707-f0cc90bd-64fa-4390-9bca-fd835d480e94.png)   
## 使用方法
在 canvas.html 使用 vscode 右键开启 live server (需安装 live server 插件) 
## 自定义热力图
1 替换图片，绑定图片的上左下右边界数据信息 至 ratioGeoPixelData 对象   
1.1 自行通过 drawLine 方法对齐边线 获得 lonPixelLeft ratioLonPixelRight ratioLatPixelTop ratioLatPixelBottom 数据    
1.2 使用如下方法得到上左下右边界数据信息 替换 ratioGeoPixelData 对象 数据   
```js
//经纬度比例数据
var ratioLonPixelLeft = lonPixelLeft / canvas2.width;
var ratioLonPixelRight = lonPixelRight / canvas2.width;
var ratioLatPixelTop = latPixelTop / canvas2.height;
var ratioLatPixelBottom = latPixelBottom / canvas2.height;

console.log("经纬度范围比例数据: ", ratioLonPixelLeft, ratioLonPixelRight, ratioLatPixelTop, ratioLatPixelBottom);
```
2.绑定对应经纬度数据的上左下右边界 至 geoData 对象   
在地图中选定经纬度信息   
3.替换对象 dotData 数据源   
