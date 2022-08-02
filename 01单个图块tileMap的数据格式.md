## 图块素材
```
0/name = "CadLevel.png 0"
0/texture = ExtResource( 1 )
0/tex_offset = Vector2( 0, 0 )
0/modulate = Color( 1, 1, 1, 1 )
0/region = Rect2( 0, 0, 32, 32 )
0/tile_mode = 0
0/occluder_offset = Vector2( 0, 0 )
0/navigation_offset = Vector2( 0, 0 )
0/shape_offset = Vector2( 0, 0 )
0/shape_transform = Transform2D( 1, 0, 0, 1, 0, 0 )
0/shape_one_way = false
0/shape_one_way_margin = 0.0
0/shapes = [  ]
0/z_index = 0

1/name = "CadLevel.png 1"
1/texture = ExtResource( 1 )
1/tex_offset = Vector2( 0, 0 )
1/modulate = Color( 1, 1, 1, 1 )
1/region = Rect2( 32, 0, 32, 32 )
1/tile_mode = 0
1/occluder_offset = Vector2( 0, 0 )
1/navigation_offset = Vector2( 0, 0 )
1/shape_offset = Vector2( 0, 0 )
1/shape_transform = Transform2D( 1, 0, 0, 1, 0, 0 )
1/shape_one_way = false
1/shape_one_way_margin = 0.0
1/shapes = [  ]
1/z_index = 0
```
- 2个单个图块

## 使用一种绘制

## TileMapData
```
tile_data = PoolIntArray( 
    0, 0, 0, 
    1, 0, 0, 
    2, 0, 0 
)
```
```
tile_data = PoolIntArray( 
    0, 1, 0, 
    1, 1, 0, 
    2, 1, 0 )
```
## 使用两种绘制
```
tile_data = PoolIntArray( 
    0, 1, 0, 
    1, 1, 0, 
    2, 1, 0, 
    
    65536, 0, 0, 
    65537, 0, 0, 
    65538, 0, 0 
)
```
`xy,tileSetID,tileID`
- `xy`=`x+y*65536`
- `tileSetId` 图块id
- `tileId`    图块集中的id 单个图块只能是0

