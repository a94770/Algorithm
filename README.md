# Front-End Coding Guidelines

<br />

### HTML编码格式规范
<br />

___

### CSS样式编码格式规范
<br />

**代码风格**

##### 1. 代码格式化

样式书写一般有两种格式：一种是紧凑格式（Compact）
```shell
.className { display: block;width: 50%; }
```
一种是紧凑格式（Expanded）
```shell
.className {
    display: block;
    width: 50%;
}
```
**团队约定：统一使用展开格式书写样式**

##### 2. 代码大小写

样式选择器，属性名，属性值关键字全部使用小写字母书写，属性字符串允许使用大小写。
```shell
/* 推荐 */
.className{
	display:block;
}
	
/* 不推荐 */
.CLASSNAME{
	DISPLAY:BLOCK;
}
```

##### 3. 选择器

- 尽量少用通用选择器 *
- 不使用 ID 选择器
- 不使用无具体语义定义的标签选择器
```shell
/* 推荐 */
.className {}
.className li {}
.className li p{}

/* 不推荐 */
*{}
#className {}
.className div{}
```

##### 4. 代码缩进

统一使用四个空格进行代码缩进，使得各编辑器表现一致（各编辑器有相关配置）
```shell
.className {
    width: 100%;
    height: 100%;
}
```

##### 5. 分号

每个属性声明末尾都要加分号；
```shell
.className {
    width: 100%;
    height: 100%;
}
```

##### 6. 代码易读性

左括号与类名之间一个空格，冒号与属性值之间一个空格
```shell
/* 推荐 */
.className {
    width: 100%;
}

/* 不推荐 */
.className{
    width:100%;
}
```

逗号分隔的取值，逗号之后一个空格
```shell
/* 推荐 */
.className {
    box-shadow: 1px 1px 1px \#333, 2px 2px 2px \#ccc;
}

/* 不推荐 */
.className{
    width:100%;
}
```