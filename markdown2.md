# 表格
  ## 创建表格
    您可以用竖线 | 和横线 - 创建表格。 横线用于创建每列的标题，而竖线用于分隔每列。 必须在表格前包含空白链接，以便其正确呈现。
    表格末尾的竖线可选。
    单元格的宽度可以不同，无需在列内准确对齐。
    例：
    
   | First Header  | Second Header 
   | - | ------ |
   | Content Cell | Content Cell   |
   | Content Cell   | Content Cell  
   
  ## 格式化表格中的内容
    您可以在表格中使用格式，如链接、内联代码块和文本样式。
    例：
    
   | Command | Description |
   | --- | --- |
   | `git status` | List all *new or modified* files |
   | `git diff` | Show file differences that **haven't been** staged |
   
    您可以在标头行中横线的左侧、右侧或两侧加入冒号 : 使表格中的文本靠左、靠右或居中对齐。
    例：
    
   | Left-aligned | Center-aligned | Right-aligned |
   | :---         |     :---:      |          ---: |
   | git status   | git status     | git status    |
   | git diff     | git diff       | git diff      |
   
    要包含竖线 | 作为单元格中的内容，请在竖线前使用 \ 。
    例：
    
   | Name     | Character |
   | ---      | ---       |
   | Backtick | `         |
   | Pipe     | \|        |
   
# 折叠部分组织信息
    您可以通过 <details> 标记创建折叠内容，使用 <summary> 标记在右侧创建展开折叠内容标签。（默认被折叠）
    例：
<details><summary>CLICK ME</summary>
<p>

    We can hide anything, even code!

```ruby
puts "Hello World"
```

</details> ```</p>

# 创建和突显代码块
  ## 围栏代码块
    通过在代码块的前后输入三反引号 ```，可创建围栏代码块。 我们建议在代码块的前后各留一个空白行，使原始格式更易辨读。
    提示：要在列表中保留格式，请确保将非围栏代码块缩进八个空格。
         要在围栏代码块中显示三重倒引号，请将其包在四个倒引号内。
    例：

````
```
function test() {
  console.log("notice the blank line before this function?");
}
```
````
  
  ## 语法突显
    您可以添加可选的语言标识符，以在围栏代码块中启用语法突显。
    使用 Linguist 来执行语言检测并选择第三方语法进行语法突显。 您可以在语言 YAML 文件中找出哪些关键词有效。
    例如，要语法突显 Ruby 代码：
    
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
puts markdown.to_html
```


# 创建图表
    您可以使用三种不同的语法在Markdown中创建图表：mermaid、geoJSON和topoJSON，以及ASCII STL。
    
  ## Mermaid
    例:使用Mermaid创建流程图。
Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
    
  ## geoJSON and topoJSON
    例：使用geojson创建地图。
```geojson
{
  "type": "Polygon",
  "coordinates": [
      [
          [-90,30],
          [-90,35],
          [-90,35],
          [-85,35],
          [-85,30]
      ]
  ]
}
```

    例：使用topoJSON创建地图。
```topojson
{
  "type": "Topology",
  "transform": {
    "scale": [0.0005000500050005, 0.00010001000100010001],
    "translate": [100, 0]
  },
  "objects": {
    "example": {
      "type": "GeometryCollection",
      "geometries": [
        {
          "type": "Point",
          "properties": {"prop0": "value0"},
          "coordinates": [4000, 5000]
        },
        {
          "type": "LineString",
          "properties": {"prop0": "value0", "prop1": 0},
          "arcs": [0]
        },
        {
          "type": "Polygon",
          "properties": {"prop0": "value0",
            "prop1": {"this": "that"}
          },
          "arcs": [[1]]
        }
      ]
    }
  },
  "arcs": [[[4000, 0], [1999, 9999], [2000, -9999], [2000, 9999]],[[0, 0], [0, 9999], [2000, 0], [0, -9999], [-2000, 0]]]
}
```

  ## ASCII STL
    例：使用ASCII STL创建3D模型。
```stl
solid cube_corner
  facet normal 0.0 -1.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 1.0 0.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
  facet normal 0.0 0.0 -1.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 1.0 0.0 0.0
    endloop
  endfacet
  facet normal -1.0 0.0 0.0
    outer loop
      vertex 0.0 0.0 0.0
      vertex 0.0 0.0 1.0
      vertex 0.0 1.0 0.0
    endloop
  endfacet
  facet normal 0.577 0.577 0.577
    outer loop
      vertex 1.0 0.0 0.0
      vertex 0.0 1.0 0.0
      vertex 0.0 0.0 1.0
    endloop
  endfacet
endsolid
```
