---
category: Components
subtitle: 文字提示
type: Data Display
title: Tooltip
---

简单的文字提示气泡框。

## 何时使用

鼠标移入则显示提示，移出消失，气泡浮层不承载复杂文本和操作。

可用来代替系统默认的 `title` 提示，提供一个`按钮/文字/操作`的文案解释。

## API

| 参数      | 说明                                     | 类型       | 默认值 |
|-----------|------------------------------------------|------------|--------|
| title     | 提示文字                                 | React.ReactNode | 无     |

### 共同的 API

以下 API 为 Tooltip、Popconfirm、Popover 共享的 API。

| 参数      | 说明                                     | 类型       | 默认值 |
|-----------|------------------------------------------|------------|--------|
| placement | 气泡框位置，可选 `top` `left` `right` `bottom` `topLeft` `topRight` `bottomLeft` `bottomRight` `leftTop` `leftBottom` `rightTop` `rightBottom` | string     | top    |
| getPopupContainer | 浮层渲染父节点，默认渲染到 body 上。`2.5.2` 之前请使用 `getTooltipContainer` | Function(triggerNode) | () => document.body |
| arrowPointAtCenter | 箭头是否指向目标元素中心，`antd@1.11+` 支持 | Boolean | `false` |
| visible   | 用于手动控制浮层显隐                     | boolean       | false  |
| onVisibleChange | 显示隐藏的回调                      | (visible) => void | 无     |
| trigger   | 触发行为，可选 `hover/focus/click`       | string        | hover  |
| overlayClassName | 卡片类名                            | string | 无     |
| overlayStyle | 卡片样式                            | object | 无     |
