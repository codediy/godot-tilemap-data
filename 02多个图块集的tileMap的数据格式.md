## 图块集 
```
0/name = "CadLevel.png 0"
0/texture = ExtResource( 1 )
0/tex_offset = Vector2( 0, 0 )
0/modulate = Color( 1, 1, 1, 1 )
0/region = Rect2( 0, 0, 512, 512 )
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

## 单个图块集绘制
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 0, 
    2, 0, 0 
)
```
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 1, 
    2, 0, 2 
)
```
`xy,tileSetID,tileID`
- `xy`=`x+y*65536`
- `tileSetId` 图块集id     从0开始
- `tileId`    图块集中的id 单个图块只能是0

## 多个图块集绘制
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 0, 
    2, 0, 0 
)
```
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 0, 
    2, 0, 0, 
    
    3, 1, 0, 
    4, 1, 0, 
    5, 1, 0 
)
```
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 0, 
    2, 0, 0, 
    
    3, 1, 0, 
    4, 1, 0, 
    5, 1, 0, 
    
    6, 1, 1, 
    7, 1, 1, 
    8, 1, 1 )
```
```
tile_data = PoolIntArray( 
    0, 0, 65536, 
    1, 0, 65536, 
    2, 0, 65536, 
    3, 0, 65536 
)
```
- `xy,tileSetID,tileID`
  - `xy`=`x+y*65536`
- `tileSetId` 图块集id     从0开始
- `tileId`    图块集中的id 单个图块只能是0
  - `tileId` = `x + y *65536`