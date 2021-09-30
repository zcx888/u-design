---
description: "用于展示日期数据的容器"

---

<!--副标题具体写法见源代码模式-->

## 简介

用于展示日期数据的容器，组合选择器可作为时间段或时间点选择器：

- 支持年份、月份切换
- 支持修改时区

## 基本构成

![此处缺图]()

<!--图片存储路径为images下新建元素名文件夹，例/images/Name/pic.png-->

| 标题栏                                                       | 容器                                               |
| :----------------------------------------------------------- | -------------------------------------------------- |
| - 展示当前年/月/日<br />- 支持快速向前/向后切换<br />- 点击可快速进入对应时间单位的选择面板 | - 展示当前最小单元的数据（如，日历下最单元为“日”） |


## 基本样式

### 种类

![此处缺图]()

<!--图片存储路径为images下新建元素名文件夹，例/images/Name/pic.png-->

| 可选范围 | 说明                                 |
| :------- | :----------------------------------- |
| 年月日   | 选择具体到“日”。默认展示今天的日期。 |
| 年月     | 选择具体到“月”。默认展示当月。       |
| 年       | 选择具体到“年”。默认展示当年。       |


### 尺寸

![此处缺图]()

<!--图片存储路径为images下新建元素名文件夹，例/images/Name/pic.png-->

|        | 尺寸 |
| :----- | :--- |
| Large  |      |
| Middle |      |
| Small  |      |



## 基本状态

![此处缺图]()

<!--图片存储路径为images下新建元素名文件夹，例/images/Name/pic.png-->

| 状态                 | 说明                   | 作用                                                         |
| :------------------- | :--------------------- | ------------------------------------------------------------ |
| 标记为今日/今月/今年 | 表示当前日期           | 区别于选中时间                                               |
| 默认初始             | --                     | --                                                           |
| 悬停                 | 鼠标划过可选数据时展示 | 暗示用户当前数据可以选择                                     |
| 选中                 | 点击后状态切换         | 表示该数据已被选中                                           |
| 禁用                 | 禁用选择               | 当前数据不可选择                                             |
| 范围外日期           | 不在当前月份内         | 补全展示上个月/下个月的日期，可点击，点击后自动切换到下一个周期 |



## 设计说明

### 原则

日历组件一般配合选择器进行使用，组合成 “时间选择器 Time Picker”或者”日期选择器 Date Picker”。

![提供时间选择器及日期选择器示意图]()

#### 1.可选范围与业务要求一致

如业务限定出明确的可选范围，应配合业务要求适时禁用向前/向后切换操作或部分日期。

![示意图]()



## 主题

| 内容 | 值           | 默认值  |
| :--- | :----------- | :------ |
| icon | icon/nothing | nothing |
| icon | icon/nothing | nothing |


## 相关文档

1. [相关文档1](https://www.ucloud.cn)
2. [相关文档2](