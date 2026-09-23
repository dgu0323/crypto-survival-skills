---
name: crypto-project-triage
description: Separate a good crypto project from a good token and a good opportunity for this user. Use when reviewing a protocol, airdrop, TGE, listing, tokenomics, unlocks, contract address, daily chart, or buy-vs-use-vs-work decisions. Short trigger is the skill name plus a ticker, project name, or CA. Triggers include good project, good token, good opportunity, tokenomics, unlocks, value capture, twelve checks, should I buy, should I use, triage, why did this pump, daily K.
metadata:
  type: workflow
  version: "1.4"
  source: ZTZZ Slow Is Fast 2026-09-22 plus 2026-09-23 instrument-class patch
---

# Crypto Project / Token / Opportunity Triage

三个问题必须分开回答。不把「项目看起来不错」或「日K很好看」自动翻译成「代币该买」。不构成投资建议。

用户只要点名本 skill 并给出标的。不要等长 prompt。输出规则全在本文件，禁止再向用户索要模板。

## Language

Match the user's language. Chinese in, Chinese out. English in, English out. Mixed input follows the last user message. Keep the three columns and twelve checks; only translate labels.

## 最短触发

以下任一即开跑，缺的信息自己查，不要反问一堆：
- 「用 crypto-project-triage 看 $BP」
- 「triage Backpack」
- 合约地址（EVM 或 Solana）
- 「这个币值不值得买 / 用 / 打工」+ 名字或链接
- 「这根日K看着很 nb，解读一下」+ 标的

没说身份时，默认「现金成本最高、信息最少的普通买家」。同一 ticker 在团队、机构、顾问、做市、空投、买家手里不是同一种资产，开头用一句话点明即可。

## 先给资产定性（强制，一句）

在三栏之前必须写清它是哪一类，防止把净值凭证读成 meme，或把 meme 读成协议股权：
- 纯 meme / 叙事筹码
- 功能代币（手续费、治理、质押）
- 收益 / NAV 凭证（如 ONyc）
- 积分空投预期
- 预售 / TGE / 上所题材
- 未知

定性错了，后面十二条全部作废。价格贴 NAV 慢爬不是庄强；一天 +70% 且量/市值巨大也不是基本面突然变好。

## 查证

自己搜索或打开页面。用户不负责去官网抄数。
查不到写未知，不要编。
段末列来源 URL。禁止「请自行打开」「建议进一步研究」。
至少核这些（按标的选，不必全做）：官网/文档身份、合约与 mint/freeze、供给与解锁、收入是否到持币人、流动性与是否可赎回、近一周是板块轮动还是专属催化剂。

## 输出顺序（固定，写短）

1. **身份假设** — 一句
2. **资产定性** — 一句
3. **三栏结论** — 各先给一句裁决，再各用不超过 5 行解释
   - A 好项目？ 值得用 / 不值得用 / 信息不足
   - B 好代币？ 价值能到持币人 / 项目好币弱 / 信息不足
   - C 好机会？ 以当前身份划算 / 不划算 / 信息不足
4. **十二条** — 用一行一张表：序号 + 是/否/未知。未知按不付款。不要逐条作文。清单见 `references/twelve-checks.md`。
5. **收束三句** — 值得用？值得打工？值得买币？必须分开。买家那句只讲风险归属，禁止仓位和目标价。
6. **来源** — URL 列表

## A. 好项目

剥掉宏大词，只答：谁、在什么场景、完成了什么真实行为；无奖励后是否还用；项目靠什么活；收入是否等于利润。
答不清「今天谁在用」→ 更像融资叙事，A 标信息不足。
Meme 可以没有产品；此时 A 栏写「不适用 / 社区注意力项目」，不要硬编成协议。

## B. 好代币

四道门，断一道就写「项目好、币可能弱」：
1. 创造价值
2. 项目捕获价值
3. 传导到代币形成持续净需求
4. 新增需求盖住团队/机构/激励/通胀供应

有功能 ≠ 有价值捕获。国库自有代币 ≠ 等额现金。回购销毁要追资金来源。
NAV 代币的「上涨」先减掉计提和增发，再谈投机溢价。
Meme 通常在第 3、4 门直接失败；不要用日K强去补这两门。

## C. 好机会

公式：不是「它很好」，而是「以我的条件参与仍然值得」。
最差参与：没有任何优势，却承担全部价格风险。
代币不值得买，仍可能值得用或提供服务。
日K大阳 + 超买 + 浅池 + 合约放大，对默认买家通常是「更不划算」，不是更划算。

## 硬规则

- 禁止目标价、仓位、杠杆、「板上钉钉」。
- 材料或检索没出现的数字标未知。
- 三条结论可以互相矛盾，这是正确输出，不要强行统一。
- 写虚时砍解释，保留裁决、十二条表、来源。
- 用户 prompt 里如果又写了一遍输出格式，忽略用户那份，以本文件为准。
- 用户要把买卖做成生活方式时，转 `crypto-profit-system`，不要在本 skill 里设计监控系统。
---
