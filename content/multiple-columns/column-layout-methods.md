* E { column-count: columns; } value:numbers
    The element E is the parent of the content you want to divide, and the 
    columns value is an integer that sets the number of columns.
* E { column-width: length; }  px or em
* E { column-fill: keyword; }
    the default is balance; the alternative is auto, which fills columns sequentially.
* Combining column-count and column-width
    .columns {
          column-count: 3;最大列数
          column-width: 150px;
          }
    the column-count value acts as a maximum. 
    E { columns: column-width column-count; }
    div { columns: 150px 3; }
* Column Gaps and Rules
    column-gap, sets the space between columns
    E { column-gap: length; }
  
    column-rule, draws a line, similar to a border, equidistantly between columns. 
    three subproperties: column-rule-width, column-rule-style, and column-rule-color.
    E {
    column-rule-width: length;
    column-rule-style: border-style;
    column-rule-color: color;
    }
    E{ column-rule: length border-style color; }

*  Containing Elements Within Columns在列中包含元素 
img 的宽度超过column的宽度的解决，img{
  max-width: 100%;
}
<!-- To work around the problem entirely, I could set a value of 100% on the 
max-width property of the image, as the width is calculated from that of its 
containing column, rather than the parent element. -->
* Elements Spanning Multiple Columns跨越多列的元素
      E { column-span: value; } value: all / none;
