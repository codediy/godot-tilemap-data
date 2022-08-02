
## tileSet
- `tile_mode` 0 单个图块 1 自动拼接 2 图块集
- `region`    图块区域
- `tile_size` 贴图大小
## tileMap的数据格式



## 地图数据
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 1, 
    2, 0, 2, 
    3, 0, 3, 
    
    65536, 0, 65536, 
    65537, 0, 65537, 
    65538, 0, 65538, 
    65539, 0, 65539 
)
```
- `mapXY`     = (x + y * 65536)
- `tileSetID` = 0
- `tileSetUV` = (u + v * 65536)
  

## 分辨率
- `mode`
  - `disable` 禁止缩放
  - `2d`      像素缩放(模糊)
  - `vieport` `viewport`缩放 最好使用这种
- `aspect`
  - `ignore`        缩放适应屏幕
  - `keep`          保持长款比
  - `keep width`    
  - `keep height`
  - `expand`        最好
- `shrink`
  - 缩放大小 
  - 4

## 项目设置
```
size
    width  = 1024
    height = 960

stretch
    mode    = viewport
    aspect  = expand
    shrink  = 4
```