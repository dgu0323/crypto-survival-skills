# Crypto Survival Skills

一套给 Grok 用的工作流 skill，用来在 Web3 / Crypto 里做位置判断，而不是喊单。

- 适用：Grok 用户技能目录（`.grok/skills/`）
- 语言：[中文 README](./README.md) · [English README](./README.en.md)

Skill 正文以中文写指令，**输出跟随用户语言**。不要再装一套英文 skill。

用户 prompt 只带材料。输出格式写在 `SKILL.md` 里，不要在对话里复述模板。

## 来源与声明

认知框架蒸馏自：

- 作者：ZTZZ（X: [@ZTZZBTC](https://x.com/ZTZZBTC)）
- 原文：[慢就是快 / Slow Is Fast](https://x.com/ztzzbtc/status/2102374831119610291)（2026-09-22）

本仓库是**第三人的工作流包装**，不是 ZTZZ 官方出品，也不是原文全文。

**不是投资建议。** 不提供代币名单、目标价、仓位或杠杆。转发请保留原文链接，不要改成「官方 skill」或「稳赚系统」。

## 四个 skill

| 目录 | 解决什么问题 | 你只需要给 |
|---|---|---|
| `crypto-incentive-decode` | 一条推文/群消息背后：谁在赚钱、谁在退出、你参与是在付谁的账 | 点名 + 链接或原文 |
| `crypto-project-triage` | 「项目不错」被直接当成「币该买」；好项目、好代币、好机会分开裁决 | 点名 + 标的或 CA |
| `crypto-niche-builder` | 只会买币、没有第二个付款者；选一个已有人付钱的生态位，落到 90 天计划 | 点名 + 可选技能/时间/正在看的叙事 |
| `crypto-profit-system` | 收入全绑在同一轮上涨、生活费和筹码混在一起；入职/加仓/FOMO 前先过结构审计 | 点名 + 你准备干什么 |

路由：

```
新叙事 / 新推文     → incentive-decode
还想参与            → project-triage
想靠行业吃饭        → niche-builder
要投入时间或现金    → profit-system
```

## 安装

目标路径：

```text
/home/workdir/.grok/skills/<skill-name>/
```

每个 skill 一个文件夹，文件夹名 = `SKILL.md` 的 `name`。`references/` 必须一起拷。装完后**新开一轮对话**再测。

### 方法 A：把 zip 丢给 Grok

```text
把这 4 个 skill 安装到 /home/workdir/.grok/skills/
保持原文件夹名。每个目录必须包含 SKILL.md 和 references/。
同名已存在先问我再覆盖。装完列出目录并校验 name 与文件夹名一致。
```

### 方法 B：GitHub

```text
从这 4 个地址安装 skill，保持原文件夹名：
https://github.com/dgu0323/crypto-survival-skills/tree/main/crypto-incentive-decode
https://github.com/dgu0323/crypto-survival-skills/tree/main/crypto-niche-builder
https://github.com/dgu0323/crypto-survival-skills/tree/main/crypto-profit-system
https://github.com/dgu0323/crypto-survival-skills/tree/main/crypto-project-triage
```

同名目录已存在时安装会失败。私有仓库需要 `GITHUB_TOKEN` 或 `GH_TOKEN`。

## 使用（短触发）

输出规则在 skill 里。下面这些已经够了。

```text
用 crypto-incentive-decode
https://x.com/……
```

```text
用 crypto-project-triage 看 $BP
```

```text
用 crypto-niche-builder
RobinHood Chain 生态
```

```text
用 crypto-profit-system
这周 $BP 翻倍，群里叫我 0.84 加仓，我没有空投
```

组合：

```text
先 decode 这条推，还想参与再用 triage。我是普通买家。
```

```text
用 niche-builder 选题，再用 profit-system 把生活费和高风险资金分开。
```

## 不要用这套 skill 做什么

- 要涨跌、币单、目标价
- 把食物链理解成全员合谋
- 把 4 个 skill 合成一个超长文件
- 和私钥、交易所 API、助记词放在一起分享

## 许可与致谢

原文版权与观点属于 ZTZZ。本包是结构化摘编，供个人学习和 Agent 工作流使用。转发请带原文链接。
