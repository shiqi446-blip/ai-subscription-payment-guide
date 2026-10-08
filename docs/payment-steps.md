---
title: ChatGPT Plus / Claude Pro / Cursor / Gemini / Midjourney 订阅付款步骤（2026-10）
description: 各 AI 服务在网页端订阅付款的步骤、要准备的东西和容易出错的地方：ChatGPT Plus 怎么付款、Claude Pro 订阅付款、Cursor Pro 付款、Gemini 订阅、Midjourney 付款。
---

# 各 AI 服务订阅付款步骤

> 整理时间：2026 年 10 月。菜单名称和价格会随版本变化，以各服务官网为准。[返回目录](index.md)

## 付款前统一准备

不管订哪一家，先把这几样准备好，能省掉大部分「Your card was declined」：

1. **一张发卡国在服务范围内的卡**（海外银行卡，或支持网页订阅的预付虚拟卡）。国内银行发的卡，包括双币卡、全币种卡，发卡国是中国，多数服务第一关就拒。
2. **账单地址**：照发卡方登记 / 提供的地址逐字段填，街道、城市、州、邮编、国家要互相对应。
3. **余额留足**：标价 + 税 + 预授权余量。$20 的订阅建议卡里至少 $25（含税地区实际扣款会高于标价）。
4. **网络出口地区**和账单地址在同一个国家，付款过程中不要切换。
5. **在网页端付款**。App 里点订阅走的是苹果 / 谷歌内购，和你绑的卡无关。

---

## ChatGPT Plus 怎么付款

- **价格**：Plus $20/月（以 [ChatGPT 官网](https://chatgpt.com/) 显示为准）。
- **收款方**：网页端通过 Stripe 收卡；iOS / Android App 也能内购，但那是另一套账单。
- **步骤**：
  1. 在浏览器登录 chatgpt.com；
  2. 点左下角头像 → 「升级套餐 / Upgrade plan」→ 选 Plus；
  3. 在付款页填卡号、有效期、CVV、持卡人姓名和账单地址；
  4. 确认订阅。扣款成功后刷新页面，左下角会显示 Plus。
- **容易出错**：
  - 已经在 App 里内购过，又在网页订一次 → 重复扣费。先在 App Store / Google Play 的订阅管理里确认；
  - 付款页的「国家」默认按网络出口地区预选，要改成账单地址所在国家；
  - 失败后连点几次「订阅」 → 触发临时风控，见 [拒付原因与解决](card-declined.md)。

## Claude Pro 订阅付款

- **价格**：Pro $20/月，年付折后约 $17/月（以 [Claude 官方价格页](https://claude.com/pricing) 为准）。
- **收款方**：网页端 Stripe；iOS / Android 可内购。
- **步骤**：
  1. 在浏览器登录 claude.ai；
  2. 左下角账户菜单 → 「Upgrade / 升级」→ 选 Pro（月付或年付）；
  3. 填卡和账单地址，确认订阅。
- **付款前先确认（客观风险提示）**：
  - 账号使用地区要在 Claude 官方的[支持地区列表](https://www.anthropic.com/supported-countries)里；
  - Claude 对付款和账号的审核比其他几家严：账单地址、常用登录地区、账号资料尽量一致，不要频繁在多个地区之间切换；
  - 2026 年有报道称部分地区的 Claude 账号被停用，用户归纳的可能因素包括数据中心 IP、卡与账单地址不一致、登录国家频繁变化；Anthropic 未公布具体原因。规则以 Claude 官方条款为准；
  - 付款被拒后不要连续换卡重试，先排查，隔一段时间再试。

## Cursor Pro 付款

- **价格**：Pro $20/月（以 [Cursor 官方价格页](https://cursor.com/pricing) 为准）。
- **收款方**：只有网页端，Stripe；没有 App 内购，所以「外区 Apple ID + 礼品卡」这条路用不了。
- **步骤**：
  1. 登录 cursor.com，进入账户设置（Dashboard / Settings）；
  2. 点「Upgrade to Pro」，跳到 Stripe 付款页；
  3. 填卡和账单地址，确认。
- **容易出错**：团队版和个人版是两套账单；用量计费的部分会在月中另外扣款，卡里要留余量。

## Gemini（Google AI Pro）订阅

- **价格**：约 $19.99/月（以 [Gemini 订阅页](https://gemini.google/subscriptions/) 和 [Google One 方案页](https://one.google.com/about/plans) 为准）。
- **收款方**：Google 自己的付款系统（Google Payments 付款资料），不是 Stripe。
- **步骤**：
  1. 用 Google 账号打开 Gemini 订阅页或 Google One；
  2. 选 Google AI Pro → 订阅；
  3. 在 Google 付款资料里添加卡片和账单地址，确认。
- **容易出错**：Google 要求**账号地区、付款资料国家、卡的发卡国、网络出口地区**尽量一致。付款资料的国家一旦建立就不能直接改，只能新建一个付款资料。

## Midjourney 付款

- **价格**：Basic $10/月，Standard $30/月起（以 [Midjourney 官网](https://www.midjourney.com/) 为准）。
- **收款方**：只有网页端，Stripe。
- **步骤**：登录 midjourney.com → 账户 / Manage Subscription → 选套餐 → 填卡。
- **容易出错**：年付一次扣款金额较大，余额要按年付总价 + 税准备。

---

## 用预付虚拟卡付款的通用流程

以 [Pink Card](https://pinkcard.cc)（利益相关：作者团队的产品）为例，其他能续充的预付卡流程类似：

1. 在官网选面值下单（网页 $110 起），付款方式以下单页为准，目前网站支持支付宝扫码自动发卡（约 1–2 分钟，另收 3% 通道费）和网站账户余额；
2. 支付宝付款成功后系统自动确认，约 1–2 分钟内卡号、有效期、CVV 和账单地址发到邮箱，不需要等客服核款；
3. 按上面对应服务的步骤绑卡，账单地址照邮件逐字段填；
4. 余额快用完前续充（每次 $5 + 5%），卡号不变，订阅不用重新绑。

费用全部列在 [费用对比表](fees.md)。不能用于 App Store / Google Play 礼品卡或内购。

---

*内容仅供参考，各服务的价格、条款以官网为准。CC BY 4.0。*
