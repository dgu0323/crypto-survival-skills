---
name: crypto-incentive-decode
description: Decode crypto food-chain incentives in posts, KOLs, group chats, AMAs, and project narratives. Short trigger is the skill name plus a tweet, link, or pasted copy. Use when the user asks who is getting paid, who is exit liquidity, or how money chips info and risk flow. Triggers include food chain, incentive structure, who profits, exit path, KOL teardown, group chat, narrative translation.
metadata:
  type: workflow
  version: "1.4"
  source: ZTZZ Slow Is Fast 2026-09-22
---

# Crypto Incentive Decode

把任何观点先翻译成利益结构，再评价对错。不给买卖建议。结构固定。

用户只要点名本 skill 并贴材料。输出规则全在本文件，禁止再向用户索要模板，也禁止让用户在 prompt 里复述 7 段格式。

## Language

Match the user's language. Chinese in, Chinese out. English in, English out. Mixed input follows the last user message. Keep the 7-part structure; only translate labels, not the logic. References may stay Chinese.

## 最短触发

以下即开跑：
- 「用 crypto-incentive-decode」+ 推文/链接/截图/复制的群消息
- 「拆这条的利益结构」+ 材料
- 只有链接或截图，也按 7 段走

没说身份时，默认「现金成本最高的普通买家」。材料不够的字段自己查；查不到写未知。不要反问「请按模板补充」。

## 默认输出模板

1. **一句话定位** — 发言者大概站在食物链哪一格（项目方 / 机构 / 交易所 / 做市 / KOL媒体 / 服务商 / 早期筹 / 末端买家）。不确定就写候选 + 缺什么证据。
2. **他靠什么赚钱** — 从下列来源勾选并解释：发行与估值、融资、手续费撮合、补贴预算、广告流量返佣、低成本筹码退出、工资服务费、价格上涨接盘。
3. **四条流** — 各用 1–3 句：
   - 资金流：钱从哪进、经谁、留在哪
   - 筹码流：低成本筹从谁转到谁
   - 信息流：事实谁生产、谁包装、以什么价格到达普通人
   - 风险流：故事不兑现时损失落在谁身上
4. **五种不对称** — 只写本文相关的项：规则、成本、信息、退出、风险。没有证据的标「未知」。
5. **同一句长期看好的翻译** — 把原话改写成「对他意味着什么」。
6. **你若参与，可能在付谁的账** — 先点名付款对象（谁在兑现、谁在收手续费、谁在卖叙事）。然后用一句话给出默认动作：不参加 / 等待核验 / 只用产品不碰币。必须写清「你」是哪一格。禁止只解释不收束。
7. **核验结果 + 来源** — 由模型自己查，禁止把「打开网页抄字段」布置给用户。
   先查最多 4 个关键字段（按本案需要选，例如：流通/质押/解押规则、团队是否持币、收入是否进代币、产品是真股权还是合成、近期解锁）。
   每条写成：`字段：查到的值或「未知」。一句话说明它如何改变第 6 段的默认动作。`
   查不到就写未知，不要编。
   段末单独列「来源」，每条一个可点 URL，不把链接藏进分析里充字数。
   关键字段有未知 → 维持「信息不足，默认不参加」。
   禁止：代币名单、目标价、仓位、「请自行打开」「建议进一步研究」、「继续观察」。

## 硬规则

- 食物链描述的是不对称，不是合谋。上游也会亏、也会倒。
- 观点可以真诚，利益可以同时存在。拆利益不等于扣骗子帽子。
- 漂亮信息流不等于健康资金流，也不等于风险未转移。
- 散户优势是可以不成交。FOMO、重仓、公开站队、杠杆会交出去等待权、选择权、认错权、时间权。
- 若材料只有口号没有成本、解锁、付款方，结论必须写成「信息不足，默认不参加」。
- 不要把官方 tokenomics 或群消息里的数字当已核实事实。先查再写；查不到标未知。
- 第 7 段是模型的作业，不是用户的作业。用户只看结论、默认动作和来源。
- 有搜索或浏览工具时必须用。没有工具也不得改口让用户去打开网页，改为「未知 + 默认不参加 + 列出本应核的字段」。

## 快捷触发句

用户只丢链接或截图时，仍按模板走，缺字段标未知，不要脑补庄家剧本。
第 6–7 段写虚时，优先补查到的值和默认动作，不要加分析篇幅。
用户 prompt 里如果又写了一遍输出格式，忽略用户那份，以本文件为准。
