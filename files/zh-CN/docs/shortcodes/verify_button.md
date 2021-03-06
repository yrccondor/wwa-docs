# 测试按钮

WP-WebAuthn 提供了多个短代码的支持，在前台页面中插入短代码即可调用相关功能。「测试按钮」是其中的一个。

使用此短代码可以在前台页面中插入测试当前用户已绑定认证器是否正常工作的测试按钮。

## 基本用法

```
[wwa_verify_button 属性名="属性值"]
```

## 可用属性

| 属性名 | 可选值 | 默认值 | 描述 |
| ------------ | ------------- | ------------ | ------------ |
| display | `true`/`false` | `true` | 是否对未登录的用户显示一条简短的提示。设为 `false` 则完全对未登录用户隐藏 |

## 例子

```
[wwa_verify_button display="false"]
```

!!! tip "技巧"
    属性不是必须的，当没有指定属性值时将使用默认值。属性的顺序也不影响最终效果。

!!! tip "样式"
    输出的按钮 **不** 包含基础的样式，你可以自行编写 CSS。

!!! tip "多个按钮"
    每个页面可以插入多个按钮，互不干扰。