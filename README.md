# Sandal for PostCSS


[sass-sandal](https://github.com/marvin1023/sandal) 的 PostCSS 版本。

使用了 CSS Next 语法，支持变量、嵌套、mixin、%等，砍掉了 Sass 中 PostCSS 一些不支持的能力。

## 覆盖默认变量

默认`variable.css`中定义了一些变量，如主色定义如下：

```css
:root {
  --primary: var(--customPrimary, #009eef);
}
```

这里使用了使用变量时传入多个参数的一个小技巧，这样你可以很方便的在另一个文件中定义`--customPrimary`变量来覆盖`--primary`的值。

具体可参考：[using-variables](https://www.w3.org/TR/css-variables/#using-variables)

## 功能介绍

## import

依赖于 PostCSS 的插件 [postcss-partial-import](https://github.com/jonathantneal/postcss-partial-import)

### 变量

使用了最新的 [CSS variable](https://caniuse.com/#feat=css-variables)，可通过 [postcss-cssnext](http://cssnext.io/) 来实现编译

### 嵌套

依赖于 PostCSS 的插件 [postcss-nested](https://github.com/postcss/postcss-nested)

### mixin

依赖于 PostCSS 的插件 [postcss-advanced-variables](https://github.com/jonathantneal/postcss-advanced-variables)

### %

依赖于 PostCSS 的插件 [postcss-extend](https://github.com/travco/postcss-extend)