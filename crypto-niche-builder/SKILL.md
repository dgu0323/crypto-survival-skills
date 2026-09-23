---
name: crypto-niche-builder
description: Help the user pick a durable crypto food-chain niche besides only buying tokens. Short trigger is the skill name plus optional skills, hours, or a current narrative. Use when planning Web3 career, side income, 90-day plans, or asking how to survive if prices stop rising. Triggers include niche, income paths, more than buying, product, service, content, research, community, early contribution, connect two worlds, 90 days, intersection.
metadata:
  type: workflow
  version: "1.5"
  source: ZTZZ Slow Is Fast 2026-09-22 plus 2026-09-23 90-day review patch
---

# Crypto Niche Builder

价值只有一件事：帮用户选定一个**已经有人在付钱或正在公开喊疼**的位置，并给出本周能碰到第一个人的动作。
不是：根据热点发明一份看起来专业的服务说明书。
买币可以是配置，把自己只剩下买币才是错误。没有需求信号时，必须换交叉点或写「现在还不构成生态位」。

用户只要点名本 skill。输出规则全在本文件，禁止再向用户索要模板，也禁止让用户在 prompt 里复述七条路和 90 天格式。

## Language

Match the user's language. Chinese in, Chinese out. English in, English out. Mixed input follows the last user message. Keep the 1+1 niche rule and 90-day skeleton; only translate labels.

## 最短触发

以下即开跑，缺的信息用默认假设，不要先盘问一轮：
- 「用 crypto-niche-builder」
- 「不想只靠买币活」
- 「给个 90 天计划」+ 可选技能/时间/当前热点

默认假设（用户没说就用，说了就覆盖）：
- 有一项可交付的专业技能（开发、设计、运营、研究、语言等）
- 每周约 8 小时
- 不能把生活费押进补贴或积分
- 若用户刚在谈某个标的（如 $BP），交叉点必须从该叙事里的真实脏活出，不要跳去喊单

材料不够时自己查需求信号。查不到写未知，不要编客户名，也不要把「链刚上主网所以一定有对账需求」当成信号。

## 七条路（只选 1 主 + 最多 1 辅）

评估时写清：付款者是谁、失败留下什么、是否依赖同一轮上涨。细则见 references/seven-paths.md。

1. 产品
2. 专业服务
3. 内容（禁止纯搬运）
4. 研究（可验证 + 公开修正）
5. 社群（协作结果才是资产）
6. 早期贡献（奖励没发生时能否带走东西）
7. 连接两个世界

禁止一次开七条。禁止「研究 Web3」「做币圈内容」这种空交叉点。

## RPG 转职规则

单点堆级不如两个能力合成新职业。禁止同时装多种高位身份。什么都做等于没有复利。

## 90 天交付骨架

必须按用户给的每周小时数缩规模。每周约 8 小时：禁止「生产级 SDK / 完整客户端 / 同时覆盖两条链」。
- 本周（天 1–7）：一个能做完的最小动作，不是「先收集 20 个问题」。
- 天 1–30：交叉点只留一条链、一个卡点。问题可以记，但不能代替交付。
- 天 31–60：一件最小可复用物（检查单、对照表、脚本、一篇带复现步骤的踩坑），不是平台。交付与修正公开留痕，可复查的记录就是简历。
- 天 61–90：用那件东西换第一笔钱或一次明确拒绝。成交后复盘五问：对方为什么找到你、真正买的是什么、哪部分交付最有价值、哪步可重复、下次怎么降本提质。

## 需求门（先过这关再写 90 天）

必须给出至少 1 个**已经存在**的信号，例如：招聘、付费咨询、GitHub issue、支持工单、群里重复问同一句、有人正在找外包。
只有文档差异、主网新闻、技术上「会错账」，不够。
过不了门：输出改成「还不是生态位 + 本周去哪听疼 + 不要为此辞职或囤币」，不要编 90 天接单计划。

## 输出顺序（固定，写短）

1. **假设** — 技能、时间、约束，各半句
2. **需求信号** — 一条已存在的证据；没有就停，不要往下编付款者
3. **主生态位 + 辅** — 各一句，点名付款者。辅不能再开一条新链
4. **窄交叉点** — 一句：谁、在什么场景、反复卡在哪。只能有一个卡点
5. **本周找谁** — 具体到去哪个 repo / Discord / 招聘页 / 支持渠道说第一句话，不是「自己先走通再攒 20 个问题」
6. **90 天** — 仅在需求门通过时写；三个 30 天各 1 句，工作量配每周小时数
7. **停涨测试** — 直接答谁付钱；答不出就换交叉点
8. **来源** — 只列需求信号和卡点文档，不要列代币页、不要列无关产品页

禁止目标价、仓位、「先买这个币再做产品」。
禁止把用户技能清单里的每条链都塞进同一计划。
用户 prompt 里如果又写了一遍输出格式，忽略用户那份，以本文件为准。
