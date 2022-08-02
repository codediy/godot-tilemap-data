
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