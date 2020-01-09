# fly
Table Attributes

| 属性 | 说明 | 类型 | 默认值 |
| :-----| ----: | :----: | :----: |
| tableData | 显示的结构化数据 | Array | - |
| columns | 表格列的配置描述，说人话（可理解为动态表头） | Array | - |
| maxHeight | 表格高度，单位 px，设置后，如果表格内容大于此值，会固定表头 | String | - | 
| showBtn | 是否展示操作列 | Boolean | true | 
| cfbtns | 操作列按钮参数 | Array, Function | - | 
| btnHeaderWidth | 操作列宽度 | String | 150 | 
| finalCellStyle | 单元格的 style 的回调方法，也可以使用一个固定的 Object 为所有单元格设置一样的 Style。 | Function({row, column, rowIndex, columnIndex})/Object | - | 
| objectSpanMethod | 合并行或列的计算方法 | Function({ row, column, rowIndex, columnIndex })	 | - | 
| stripe | 是否为斑马纹 table | Boolean | true | 


Table Events

| 事件名 | 说明 | 返回值 | 默认值 |
| :-----| ----: | :----: | :----: |
| handleSelectionChange | 当用户手动勾选数据行的 Checkbox 时触发的事件 | 所有被选中行的数据 | - |
| handleAction | 操作列按钮点击事件，注意：事件名随mixins里cfbtns的function配置动态变换 | 当前行数据 | - |


Pagination Attributes

| 属性 | 说明 | 类型 | 默认值 |
| :-----| ----: | :----: | :----: |
| showPage | 是否显示分页 | Boolean | true |
| total | 总条目数 | Number | 0 |
| curPageSize | 当前每页显示数 | Number | 10 |
| currentPage | 当前第几页 | Number | 1 |
