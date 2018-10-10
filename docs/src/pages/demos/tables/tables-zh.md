---
title: Table React component
components: Table, TableBody, TableCell, TableFooter, TableHead, TablePagination, TableRow, TableSortLabel
---
# 表格

<p class="description">表格用于展示数据集。表格可以被充分定制化。</p>

[数据表格](https://material.io/design/components/data-tables.html)以一种一目了然地方式显示信息，这便于用户发现某些模式和要义。 表格可以被内嵌在主要内容中，如卡片。

数据表可以包括: -对应的数据可视化展现 -导航 -用于查询和操作数据的工具

在包含工具时, 应将它们直接放在表格的上方或下方。

## 结构

数据表的顶部是标题行，给出各列的名称，后续的各行是表格数据。

如果用户需要选择或操作数据, 则每一行应包含有复选框。

出于可访问性考虑, 表格第一列设置为 `<th>` 元素, 其 `scope` 属性指定为 `"row"`。 This enables screen readers to identify a cell's value by it's row and column name.

## 简单表格

A simple example with no frills.

{{"demo": "pages/demos/tables/SimpleTable.js"}}

## 排序&筛选

This example demonstrates the use of `Checkbox` and clickable rows for selection, with a custom `Toolbar`. It uses the `TableSortLabel` component to help style column headings.

The Table has been given a fixed width to demonstrate horizontal scrolling. In order to prevent the pagination controls from scrolling, the TablePagination component is used outside of the Table. (The ['Custom Table Pagination Action' example](#custom-table-pagination-action) below shows the pagination within the TableFooter.)

{{"demo": "pages/demos/tables/EnhancedTable.js"}}

## 自定义表格分页行为

The `Action` property of the `TablePagination` component allows the implementation of custom actions.

{{"demo": "pages/demos/tables/CustomPaginationActionsTable.js"}}

## 自定义表格

You can customize the look and feel of the table by overriding the styles of the `TableCell` component.

{{"演示": "pages/demos/badges/SimpleBadge.js"}}

## Advanced use cases

For more advanced use cases you might be able to take advantage of: - [dx-react-grid-material-ui](https://devexpress.github.io/devextreme-reactive/react/grid/) A data grid for Material-UI with paging, sorting, filtering, grouping and editing features ([custom license](https://js.devexpress.com/licensing/)). - [mui-datatables](https://github.com/gregnb/mui-datatables) Responsive data tables for Material-UI with filtering, sorting, search and more. - [material-table](https://github.com/mbrn/material-table) DataTable based on table component with additional features like search, filtering, sorting and much more.