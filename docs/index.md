---
title: AI 订阅付款指南：ChatGPT Plus / Claude Pro / Cursor / Gemini 付款失败怎么办
description: 国内卡订阅 ChatGPT Plus、Claude Pro、Cursor、Gemini、Midjourney 被拒的原因，各付款方式的费用对比，以及「Your card was declined」排障清单。2026 年 10 月更新。
---

# AI 订阅付款指南（2026-10 更新）

**How to pay for ChatGPT Plus, Claude Pro, Cursor, Gemini and Midjourney when your card is declined.** [English FAQ →](faq-en.md)

用国内银行卡（包括双币卡、全币种卡）订阅 ChatGPT Plus、Claude Pro、Cursor Pro、Gemini、Midjourney，经常看到「Your card was declined」。这里把原因、付款方法、费用和排障步骤拆成几篇短文，按需要看：

| 文章 | 回答的问题 |
|---|---|
| [Claude Code 订阅付款](claude-code-subscription-payment.md) | Claude Code 走 Pro / Max 订阅还是 API 按量，各种付款方式的门槛和费用 |
| [ChatGPT 订阅怎么付款](chatgpt-subscription.md) | ChatGPT Plus / Pro 网页端、iOS、安卓三种订阅渠道，国内能用的付款办法对比 |
| [怎么有一张海外信用卡](overseas-credit-card.md) | 双币卡、港卡、海外银行卡、预付虚拟卡、礼品卡的区别和门槛 |
| [各 AI 服务付款步骤](payment-steps.md) | ChatGPT Plus / Claude Pro / Cursor / Gemini / Midjourney 分别在哪里付款、要准备什么 |
| [Claude Pro / ChatGPT Plus / Cursor 付款失败排查](claude-chatgpt-cursor-payment-failed.md) | 三家各自特有的付款失败原因：地区限制、预授权、按量计费补扣、续费失败 |
| [常见拒付原因与解决](card-declined.md) | 看到「Your card was declined」「card not supported」「邮编不正确」该怎么办 |
| [支付宝提示「单笔跨境金额超过上限」怎么办](alipay-cross-border-limit.md) | 付海外网站 / AI 订阅 / 预付卡时被支付宝拦下：会不会扣钱、为什么别人能付、拆单和换付款方式的代价 |
| [Grok / SuperGrok 怎么订阅付款](Grok-SuperGrok-订阅付款.md) | SuperGrok 各档价格、网页 / App / X 会员三个入口、国内卡被拒原因和排查顺序 |
| [ChatGPT 代充靠谱吗](ChatGPT-代充靠谱吗.md) | 代充四种做法的风险、六条能自己核的判断标准、用过代充后怎么收回登录、不代充的付款方式 |
| [Vercel 怎么付款](Vercel-付款.md) | Vercel Pro / v0 绑卡、Marketplace 数据库单独扣款、扣款失败多久暂停部署、被拒排查 |
| [Suno 怎么订阅付款](Suno-订阅付款.md) | Suno Pro / Premier 价格和积分、网页和 App 内购怎么选、绑卡被拒排查 |
| [OpenRouter 怎么充值](OpenRouter-充值.md) | 支付宝直接充还是绑卡、5.5% 手续费怎么算、自动充值为什么只能绑卡、24 小时退款和额度过期、付款失败排查 |
| [ElevenLabs 怎么付款](ElevenLabs-付款.md) | Starter / Creator / Pro 价格和积分结转、预付卡为什么可能被拒、首月折扣结束后的续费失败、14 天退款条件 |
| [Gamma 怎么付款](Gamma-付款.md) | Gamma Plus / Pro / Ultra 怎么选、只收银行卡、含税扣款和升级补差价、被拒排查、3 天退款规则 |
| [ChatGPT Plus / Claude Pro 订阅被拒报错对照](订阅被拒-报错对照.md) | Your card was declined、card_not_supported、do_not_honor、incorrect_zip、3D Secure 等报错各是什么意思、该怎么办，6 个按顺序做的自查办法，我们卡上失败原因分布 |
| [X（推特）Premium 怎么付款](X-Premium-付款.md) | Basic / Premium / Premium+ 价格、网页和 App 内购的区别、每日购买次数上限、续费失败和退款规则 |
| [Figma 怎么付款](Figma-付款.md) | Professional 三种席位价格、绑卡步骤、被拒原因、续费失败 21 天重试后锁成只读的补救 |
| [Replicate 怎么付款](Replicate-付款.md) | 预付额度一年有效不退款、绑卡 $0 验证、自动充值门槛、被拒排查、怎么买手续费占比低 |
| [费用对比表](fees.md) | 各种付款方式一年下来多花多少钱 |
| [English FAQ](faq-en.md) | Paying for AI subscriptions with a virtual card, in English |

完整长文（方法逐项对比 + 决策表）在仓库首页：[README](https://github.com/shiqi446-blip/ai-subscription-payment-guide#readme)。更新记录见 [CHANGELOG](https://github.com/shiqi446-blip/ai-subscription-payment-guide/blob/main/CHANGELOG.md)。

## 三句话结论

1. **大多数「卡里有钱却被拒」是因为发卡行国家不在服务范围内**，不是余额或操作问题。国内银行发的卡，不管是不是双币卡，基本都过不了第一关。
2. **在网页端订阅，不要在 App 里订**：App 内购走苹果 / 谷歌，和你绑的卡无关。
3. **被拒后不要连续重试**：先删卡、逐项核对、隔几个小时再绑。连续失败会被风控记住，很多预付卡失败也收手续费。

## 利益相关

本站作者团队做 [Pink Card](https://pinkcard.cc)（预付虚拟卡），它只是几种付款方法之一。费用在[费用对比表](fees.md)里照实列出，包括它比零月费方案贵的地方。其余内容尽量中立，各服务的价格和条款以官方页面为准。

---

*内容仅供参考，不构成金融建议。CC BY 4.0。*
