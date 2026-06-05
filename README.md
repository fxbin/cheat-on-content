# Cheat on Content · 小红书内容校准版

> 这是 `cheat-on-content` 的小红书 / 数字产品内容适配版。  
> 核心不是“让 AI 替你写爆款”，而是把每一篇笔记变成一次可记录、可预测、可复盘、可进化的内容实验。

## 它解决什么问题

很多内容创作者的问题不是不会发，而是：

- 每条笔记都凭感觉判断好坏；
- 发完只看点赞、收藏、浏览，却没有沉淀判断标准；
- 事后复盘容易“合理化”，很难知道自己发布前到底判断准不准；
- 做资料包、小红书店铺、课程产品时，流量数据和成交信号没有连起来。

这个 Skill 的闭环是：

```text
选题入池 → 发布前评分 → 盲预测 → 发布登记 → T+3d 复盘 → 升级 rubric
```

它更像一个“内容运营校准系统”，不是普通标题生成器。

## 这个 fork 新增了什么

本 fork 针对以下场景做了适配：

1. 小红书图文笔记；
2. 数字资料包推广；
3. HSK / 对外汉语教学资料；
4. 幼小衔接、拼音、识字资料；
5. 外贸资料库、轻量知识产品；
6. 有 IP 角色承接的教育内容账号。

新增内容：

- `docs/XHS_CONTENT_CALIBRATION_CN.md`：小红书内容校准工作流说明；
- `starter-rubrics/xhs-digital-product.md`：小红书数字产品专用评分公式；
- `templates/xhs-content-project/`：可直接复制到内容项目的模板；
- `skills/cheat-xhs-init/SKILL.md`：小红书项目初始化子 skill。

## 快速开始

安装后，在你的内容项目目录里说：

```text
初始化小红书内容校准
```

或者：

```text
初始化 cheat-on-content，用小红书数字产品模式
```

初始化后，建议目录结构如下：

```text
my-xhs-content/
├── rubric_notes.md
├── WORKFLOW.md
├── STATUS.md
├── .cheat-state.json
├── candidates.md
├── scripts/
├── predictions/
├── posts/
├── reports/
└── samples/
```

## 日常使用

```text
打分这篇 scripts/2026-06-05_hsk_card.md
启动预测 scripts/2026-06-05_hsk_card.md
已发布 小红书链接是 ...
复盘 posts/2026-06-05_hsk_card/
推荐选题
升级 rubric
状态
```

## 小红书复盘看什么

不要只看阅读量。对数字产品账号来说，更重要的是：

- 封面点击力；
- 收藏率；
- 评论里的真实需求；
- 是否有人问“怎么领 / 怎么买 / 有链接吗”；
- 商品点击；
- 私信数；
- 成交或加购信号；
- 是否吸引了目标买家，而不是泛流量。

## 推荐的第一批内容项目

对当前使用者，建议优先建立 3 个项目：

1. `xhs-hsk-products`：HSK 3.0 字卡、字帖、PPT、商品详情页；
2. `xhs-kids-literacy`：拼音、识字、幼小衔接、橙橙狐资料；
3. `xhs-productization-notes`：把技能产品化、资料库、轻量数字产品方法论。

每个项目单独维护自己的 `rubric_notes.md`，不要混在一起。

## 原始方法论保留

这个 fork 仍然保留原项目的核心原则：

1. **盲预测**：发布前写预测，发布后不能改预测段；
2. **全量重打**：升级评分公式前，要用历史样本验证新公式；
3. **rubric 是工作台**：被数据推翻或吸收的旧观察要删掉，不要堆成考古笔记。

## 安装

```bash
git clone https://github.com/fxbin/cheat-on-content.git
cd cheat-on-content
bash install.sh
```

Codex 用户可以使用：

```bash
bash install.sh --codex
```

## License

MIT。原项目来自 `XBuilderLAB/cheat-on-content`，本 fork 主要增加小红书 / 中文数字产品运营适配层。
