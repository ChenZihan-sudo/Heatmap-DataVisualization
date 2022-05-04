# Heatmap-DataVisualization
简易实现热力地图数据可视化     

![image](https://user-images.githubusercontent.com/64928288/166636707-f0cc90bd-64fa-4390-9bca-fd835d480e94.png)      
## 自定义热力图
1.替换图片，绑定图片的上左下右边界数据信息 至 ratioGeoPixelData 对象
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
