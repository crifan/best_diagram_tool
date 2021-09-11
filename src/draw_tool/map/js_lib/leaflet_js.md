# leaflet.js

* `leaflet.js`
  * 是什么：js库
  * 概述：一款能实现交互式地图功能的主流的js库
  * 资料
    * 主页
      * Leaflet - a JavaScript library for interactive maps
        * https://leafletjs.com/
          * ![leafjs_homepage](../../assets/img/leafjs_homepage.jpg)
    * 教程
      * Tutorials - Leaflet - a JavaScript library for interactive maps
        * https://leafletjs.com/examples.html
    * API文档
      * Documentation - Leaflet - a JavaScript library for interactive maps
        * https://leafletjs.com/reference-1.7.1.html
  * 示例代码
    ```js
    var map = L.map('map').setView([51.505, -0.09], 13);

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);

    L.marker([51.5, -0.09]).addTo(map)
        .bindPopup('A pretty CSS3 popup.<br> Easily customizable.')
        .openPopup();
    ```

## Python版leaflet

* Python版leaflet = leaflet的Python的接口
  * `Folium`
    * 概述：一个基于`leaflet.js`的Python地图库
    * GitHub
      * python-visualization/folium: Python Data. Leaflet.js Maps.
        * https://github.com/python-visualization/folium
    * 文档
      * Folium — Folium 0.12.1 documentation
        * https://python-visualization.github.io/folium/
      * 快速上手
        * Quickstart — Folium 0.12.1 documentation
          * https://python-visualization.github.io/folium/quickstart.html
            * ![folium_marker_icon](../../assets/img/folium_marker_icon.jpg)
    * 示例
      * Jupyter Notebook Viewer
        * https://nbviewer.jupyter.org/github/python-visualization/folium/tree/master/examples/
          * 彩色地图
            * https://nbviewer.jupyter.org/github/python-visualization/folium/blob/master/examples/Colormaps.ipynb
              * ![map_folium_color_us](../../assets/img/map_folium_color_us.jpg)
