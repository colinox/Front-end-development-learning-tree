<!-- TOC -->

- [表单中Readonly和Disabled的区别](#%e8%a1%a8%e5%8d%95%e4%b8%adreadonly%e5%92%8cdisabled%e7%9a%84%e5%8c%ba%e5%88%ab)

<!-- /TOC -->

## 表单中Readonly和Disabled的区别

`readonly`和`disabled`是用在表单中的两个属性，它们都能够做到使用户不能够更改表单域中的内容。但是它们之间有着微小的差别，总结如下：

`readonly`只针对`input(text / password)`和`textarea`有效，而disabled对于所有的表单元素都有效，包括`select`, `radio`, `checkbox`, `button`等。

但是表单元素在使用了`disabled`后，会导致绑定事件失效，当我们将表单以POST或GET的方式提交的话，这个元素的值不会被传递出去，而`readonly`会将该值传递出去（这种情况出现在我们将某个表单中的`textarea`元素设置为`disabled`或`readonly`，但是`submit` `button`却是可以使用的）。

`disabled`和`readonly`这两个属性有一些共同之处，比如都设为true，则form属性将不能被编辑，往往在写js代码的时候容易混合使用这两个属性，其实他们之间是有一定区别的。

如果一个输入项的`disabled`设为true，则该表单输入项不能获取焦点，用户的所有操作（鼠标点击和键盘输入等）对该输入项都无效，最重要的一点是当提交表单时，这个表单输入项将不会被提交。

而readonly只是针对文本输入框这类可以输入文本的输入项，如果设为true，用户只是不能编辑对应的文本，但是仍然可以聚焦焦点，并且在提交表单的时候，该输入项会作为form的一项提交。

设置为`disabled`的`input`将会有下面的限制：

- 不能接收焦点
- 使用tab键时将被跳过
- 可能不是successful的

设置为`readonly`的`input`将会有下面的限制：

- 可以接收焦点但不能被修改
- 可以使用tab键进行导航
- 可能是successful的

这两个属性在效果和使用上的区别：

1. readonly是要锁定这个控件，通过在界面上无法修改他（但是通过javascript可以修改他）。
2. disabled和readonly有相同的地方也是可以锁定这个控件用户不能改变他的值，但是disabled的更彻底一些，他是要使你完全不能使用他，包括改变他的背景颜色（不信，你去修改一个被disabled掉的input文本框，你发现你是徒劳），如果是checkbox则不能选中他。
3. 所有控件都有disabled 属性，但是不一定有readonly属性，如select 下拉框。点击被readonly掉的按钮照样可以触发事件，但是被disabled掉的按钮就无法使用了不管上面有没有事件。