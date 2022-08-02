## data数据格式
```
```
- `mapXY,tileSetId,tileSetUV`
  - `mayXY`      地图的xy坐标   x + y * 65536
  - `tileSetId`  图块集id   
  - `tileSetXY`  图块集的uv坐标 u + v * 65536

## 图块集
```
0/name = "CadLevel.png 0"
0/texture = ExtResource( 1 )
0/tex_offset = Vector2( 0, 0 )
0/modulate = Color( 1, 1, 1, 1 )
0/region = Rect2( 0, 0, 128, 64 )
0/tile_mode = 2
0/autotile/icon_coordinate = Vector2( 0, 0 )
0/autotile/tile_size = Vector2( 32, 32 )
0/autotile/spacing = 0
0/autotile/occluder_map = [  ]
0/autotile/navpoly_map = [  ]
0/autotile/priority_map = [  ]
0/autotile/z_index_map = [  ]
0/occluder_offset = Vector2( 0, 0 )
0/navigation_offset = Vector2( 0, 0 )
0/shape_offset = Vector2( 0, 0 )
0/shape_transform = Transform2D( 1, 0, 0, 1, 0, 0 )
0/shape_one_way = false
0/shape_one_way_margin = 0.0
0/shapes = [  ]
0/z_index = 0
```
- tile_mode = 2 图块集
- region        图块像素集
- tile_size     贴图大小

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