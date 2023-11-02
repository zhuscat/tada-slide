---
theme: default
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
transition: slide-left
title: 基于 LLM 的服装管理/搭配系统
mdc: true
---

# 基于 LLM 的服装管理/搭配系统

饼：All-in-One 物品管理系统

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# 📹 先看个视频

<video controls>
  <source src="/assets/presentation.mp4" type="video/mp4">
</video>

---

# 🙋 问题概述

- 👔 如何对自己的服装进行规划...
- 😩 忘记自己有什么衣服
- 🤔 烦恼自己今天应该穿什么

<!--
Here is another comment.
-->

---
layout: center
class: text-center
transition: fade-out
---

# 上海秋冬之交，路上有人穿羽绒服、有人穿短袖，出门前无法迅速决策我应该穿什么

---
layout: center
class: text-center
transition: fade-out
---

# 双十一买衣服，买回来之后发现衣柜中已经有同类的衣服了，浪费💰

---
layout: center
class: text-center
transition: fade-out
---

# 打工人搬家尽是衣？如何断舍离

---
layout: default
---

# 更进一步的

- 🍕 食品管理，过期、补货...
- 🔋 小物件管理，电池、充电线...
- 🤩 一切物件...

---

# 同类产品

<div class="flex gap-x-16px">
  <img src="/assets/dada.jpg" class="w-184px rounded-lg shadow" />

  <img src="/assets/jinjianyichu.jpg" class="w-184px rounded-lg shadow" />

  <img src="/assets/xindongyichu.jpg" class="w-184px rounded-lg shadow" />

  <img src="/assets/haodahezi.jpg" class="w-184px rounded-lg shadow" />
</div>

---
layout: default
---

# 同类产品

<div class="flex gap-x-16px">
  <img src="/assets/wodewupin.jpg" class="w-184px rounded-lg shadow" />

  <img src="/assets/guoqila.jpg" class="w-184px rounded-lg shadow" />
</div>

---

# 分析

## 面向用户群体
- 家中衣物（物品）比较多的人
- 对物品有自己规划的人
- 期望能有一个穿搭顾问，买衣顾问...
- 对将所有衣物（物品）进行记录有特殊癖好的人...

## 规模

比如尽简衣橱，今日 App Store 生活类排名是 65

如果能够做到非常好的体验，并且在保持体验的情况下把品类从服装扩展出去，做到物品 All-in-One，应该能够有一定的市场规模

---
layout: two-cols
---

# 我的作品

<div class="flex">
<div class="flex flex-col items-center">
  <img src="/assets/tada-icon.svg" class="w-108px h-108px" />
  <span class="font-semibold text-xl">Tada</span>
  <img src="/assets/slogan.gif" class="w-200px" />
</div>
</div>

::right::

# 已实现用例

- 基础的登录/注册，个人偏好信息录入
- 衣物快捷录入
- 基于 LLM 的推荐/服装查询/收藏（使用 ReAct 的方式）

---
layout: two-cols
---

# 录入

## 设想

- 拍照、扫码、已有数据选取
- 对图片进行识别，比如利用分类模型、或者 GPT4 对图片进行描述、颜色提取、抠图等等，用最小成本完成录入信息的提取

::right::

<img src="/assets/add_cloth.jpeg" class="w-200px rounded-lg shadow mt-56px ml-32px" />

---

# 对话

提供一种对话式的交互方式，在拓展到其他类目的时候，也许能提供一种通用的交互形式。可以问各种问题，比如数据查询、穿搭推荐、收藏...

<div class="flex gap-x-16px">
  <img src="/assets/chat-1.png" class="w-184px rounded-lg shadow" />
  <img src="/assets/chat-2.png" class="w-184px rounded-lg shadow" />
  <img src="/assets/chat-3.png" class="w-184px rounded-lg shadow" />
</div>


---

# 对话 Case

这是我**设想**的一些对话 Case

- 早上起床，问：今天穿什么？这周穿什么...
- 推荐了一个合适穿搭，帮我收藏...
- 帮我找一件已经录入过的衣服是否存在...
- 我在店里买衣服，看到一件衣服，拍照，然后询问我是否应该买这件衣服？这件衣服与我其他衣服该如何搭配？等等

---
layout: center
---

# Demo

---

# 做的过程中的发现的一些问题

- 一个强大的 LLM 是否能够提供或者如何才能够提供符合个人美学的搭配
- 是否能够或者如何能够根据个人身体的情况进行合理的搭配
- 输出不完全可控的问题

---

# 更多功能的想法

- 个人信息录入，更加智能化，比如拍一张照片，进行身材分析等等；比如根据一些设备或者预设问题，分析个人怕冷、怕热之类的信息
- 衣橱/物品管理，基于自然语言的筛选器：比如创建一个筛选，请将我的衣服按颜色进行分类
- ...

---

# 畅想

- 作为一个 All-in-One 的物品管理，与我们现有标记、C2C 结合，数据打通...
- 当这个系统能够管理用户的所有物品，可以进一步的进行更多的专属个性化推荐

---
layout: center
---

# Thanks! 请给我投票，🙏💗🙏