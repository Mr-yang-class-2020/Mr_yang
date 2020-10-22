# table

在表格内，通过行与列来创建表格。tr代表行。td代表列，也叫单元格

>  创建一个一行2列的表格

```html
<table>
	<tr>
		<td>
				1
		</td>
		<td>
				2
		</td>
	</tr>
</table>
```





默认状态下，table制作出来的表格没有基本表格出现的边框线等,所以，我们可以为table添加如下的属性---`border`



### border属性

table的border属性用于为table元素添加边框，值为数字，单位可有可无

```html
<table border='1'>
	<tr>
		<td>
			1
		</td>
		<td>
			2
		</td>
    </tr>
</table>
```



border只作用于 table 和 td 这两个元素  不能为tr提供边框效果。



### width 和 height



```html
<table border='1' width='800px' height='400'>
	<tr>
		<td  width='200'>
				1
		</td>
		<td>
				2
		</td>
	</tr>
</table>
```

注意：行是没有宽度的，行只有height，tr的宽度永远等于表格的宽度，当tr的数量大于1行的时候，tr是可以设置高度的。

对于table内的单元格设置宽度和高度的时候，通常为tr设置高度 为td设置宽度

> `td改变列宽       tr改变行高`



### align 水平排列属性

> align = 'left/center/right'

该属性对于table/tr/td都存有不同的显示效果

对于table而言。align的值，改变了当前table表格的水平位置

对于tr而言。align的值，改变当前行内 所有单元格的值的位置

对于td而言。align的值。改变当前单元格的值的位置



### valign 垂直排列属性

> valign='top/middle/bottom'

对于tr而言。valign的值，改变当前行内 所有单元格的值的位置

对于td而言。valign的值。改变当前单元格的值的位置



### table 表格的cellpadding

cellpadding 相当于为当前的所有单元格 内部填充一个值（四个方向）

> 不太适合在开发中使用，局限性太大。



### table 表格的cellspacing 

用于吧table的边框和单元格之间的边框合并成一条线









在创建表格的时候，一定先定义thead 和tfoot,因为除了这两个元素内包含的tr之外。其他的tr都会默认的添加到tbody里面