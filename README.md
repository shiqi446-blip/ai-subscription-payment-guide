# ChatGPT Plus / Claude Pro / Cursor / Gemini 付款失败怎么办：AI 订阅付款方法对比

**How to pay for ChatGPT Plus, Claude Pro, Cursor, Gemini and Midjourney when your card is declined — methods, fees and a troubleshooting checklist.**

> 用国内银行卡（包括双币卡、全币种卡）订阅 ChatGPT Plus、Claude Pro、Cursor Pro、Gemini、Midjourney，经常看到「Your card was declined」或「付款失败」。本地卡经常被拒的海外用户也一样。这份指南讲清楚被拒的原因，对比 App 内购、虚拟卡等几种付款方式的优缺点和费用，最后附一份「付款被拒」排障清单。
>
> 整理时间：2026 年 10 月。商户规则和各家费率变化很快，表里的数字请以各自官网为准。发现过时的内容欢迎提 Issue / PR。

**English summary at the bottom · 英文摘要在文末 · 网页版（更易读）：<https://shiqi446-blip.github.io/ai-subscription-payment-guide/>**

**分篇 FAQ（docs/）**：

- [各 AI 服务付款步骤：ChatGPT Plus / Claude Pro / Cursor / Gemini / Midjourney](docs/payment-steps.md)
- [Claude Pro / ChatGPT Plus / Cursor 付款失败原因与排查](docs/claude-chatgpt-cursor-payment-failed.md)
- [Your card was declined：常见拒付原因与解决](docs/card-declined.md)
- [AI 订阅付款方式费用对比表（含一年总成本算例）](docs/fees.md)
- [English FAQ: paying for AI subscriptions with a virtual card](docs/faq-en.md)
- [更新记录 CHANGELOG](CHANGELOG.md)

> **利益相关**：本仓库作者团队在做 Pink Card（一种预付虚拟卡），它是下面对比的方法之一，单独放在第 4 节，费用照实写。其余部分尽量保持中立，不点名推荐也不点名贬低任何一家。

---

## 目录

1. [先搞懂：为什么你的卡付不了](#1-先搞懂为什么你的卡付不了)
2. [各服务的收款方式一览](#2-各服务的收款方式一览)
3. [付款方法对比](#3-付款方法对比)
4. [Pink Card（利益相关）](#4-pink-card利益相关)
5. [付款被拒排障清单](#5-付款被拒排障清单)
   - [5.5 Claude Pro / ChatGPT Plus / Cursor 付款常见失败原因与排查](#55-claude-pro--chatgpt-plus--cursor-付款常见失败原因与排查)
6. [Claude Pro 单独说明](#6-claude-pro-单独说明)
7. [怎么选：一张决策表](#7-怎么选一张决策表)
8. [English Summary](#english-summary)
9. [延伸阅读：分篇 FAQ](#延伸阅读分篇-faq)

---

## 1. 先搞懂：为什么你的卡付不了

> 关键词：ChatGPT Plus 付款被拒、Claude Pro 订阅付款失败、Cursor 国内卡被拒、Your card was declined

ChatGPT、Claude、Cursor、Midjourney 的网页端基本都通过 Stripe 收款，Gemini 走 Google 自己的付款系统。不管哪家，每笔扣款大致会核对这几项：

| 检查项 | 说明 | 国内卡的典型情况 |
|---|---|---|
| 发卡行所在国家 | 商户会按卡号前几位（BIN）判断发卡行国家，不在服务范围内的直接拒 | 国内银行发的 Visa / Mastercard，包括双币卡、全币种卡，发卡国都是中国，第一关就过不去 |
| 卡的类型 | 借记 / 贷记 / 预付。部分商户会拦截某些预付卡段 | — |
| 账单地址（AVS） | 填写的地址、邮编要和发卡方登记的一致 | 国内卡没有可用的海外账单地址 |
| 网络出口地区 | 付款时的网络出口地区和账单地址国家不一致，会被风控加分 | — |
| 3DS 验证 | 部分交易要求发卡行短信或 App 验证 | 跨境 3DS 经常收不到或验证失败 |
| 余额 / 额度 | 含税金额、预授权冻结都要够 | — |

结论：**大多数「卡里明明有钱却被拒」，问题出在发卡行国家，不在余额，也不在操作。** 换一张发卡国在服务范围内的卡，是绝大多数方法的本质。

---

## 2. 各服务的收款方式一览

> 关键词：ChatGPT Plus 怎么付款、Claude Pro 订阅付款方式、Gemini 订阅付款、Cursor Pro 付款、Midjourney 付款

| 服务 | 常见套餐（月付，美元） | 网页端收款 | App 内购 | 备注 |
|---|---|---|---|---|
| ChatGPT Plus | $20 | Stripe，信用卡 / 借记卡 | iOS / Android 可内购 | 网页订阅和 App 内购是两套账单，别重复订 |
| Claude Pro | $20（年付折后约 $17/月） | Stripe | iOS / Android 可内购 | 审核较严，见第 6 节 |
| Gemini（Google AI Pro） | 约 $19.99 | Google 付款资料 | Google Play | 账号地区、卡的地区、网络出口地区要一致 |
| Cursor Pro | $20 | Stripe | 无 | 只能网页付款 |
| Midjourney | Basic $10 / Standard $30 起 | Stripe | 无 | 只能网页付款 |

> 价格会变，带税地区实际扣款会高于标价。

---

## 3. 付款方法对比

> 关键词：AI 订阅虚拟卡、AI subscription virtual card、App 内购、代充

### 3.1 总表

| 方法 | 适用服务 | 一次性成本 | 持续成本 | 门槛 | 稳定性 | 主要风险 |
|---|---|---|---|---|---|---|
| 海外实体卡（本人名下） | 全部 | 开户成本 | 通常无额外费用 | 高：要有海外身份或账户 | 最高 | 几乎没有，前提是人或账户真在海外 |
| 外区 Apple ID + App Store 礼品卡 | 有 iOS App 的：ChatGPT、Claude、Gemini 部分套餐 | 礼品卡溢价 | 每月买卡，溢价持续 | 中：要会注册外区账号 | 中 | 礼品卡来源、账号地区限制、无法用于网页端 |
| 朋友代付 | 全部 | 无 | 人情 | 低 | 取决于朋友 | 账单在别人卡上，退款、换套餐都被动 |
| 交易平台发行的联名卡 | 走 Stripe 的服务大多可以 | 开卡费低或免费 | 费率低，多为 1% 左右，通常零月费 | 中到高：要先在该平台开户、做身份认证、换好美元资产 | 中 | 要多开一个平台账户；部分地区不发卡 |
| 支持支付宝等国内方式入金的预付卡 | 走 Stripe 的服务大多可以 | 开卡费几美元到 $20 不等 | 充值费 3% 上下，部分有年费 | 低到中：多数要身份认证 | 中 | 这类平台近两年关停不少，选之前看运营时间和退款口碑 |
| 一次性虚拟卡 | 单次付款 | 每张一笔费用 | 每月重新买、重新绑卡 | 低 | 低到中 | 续费时卡已作废，订阅会中断 |
| 第三方代充 / 合租账号 | ChatGPT 为主 | 无 | 按月付给代充方，常见 ¥130–170/月 | 最低 | 低 | 账号密码交给别人；合租违反多数服务条款；对方随时可能改密码 |

### 3.2 逐项说明

#### 海外实体卡

- **优点**：最稳，所有服务都能付，没有额外费用，出问题有银行兜底。
- **缺点**：门槛最高，需要海外身份、地址或账户。留学、海外工作的人首选。
- **注意**：如果你人在海外，但卡是国内发的，仍然会在「发卡行国家」这一关被拒。在当地开一张借记卡最省事。

#### 外区 Apple ID + App Store 礼品卡

- **做法**：注册一个服务可用地区的 Apple ID，购买该地区的 App Store 礼品卡充值，然后在 iOS App 里内购订阅。
- **优点**：不需要任何卡；礼品卡可以用常见的国内付款方式从第三方买到。
- **缺点**：
  - 只能在 iOS App 内订阅，Cursor、Midjourney 这类没有 App 内购的服务用不了。
  - 礼品卡基本从第三方购买，有溢价，来源也参差不齐。
  - 一个 Apple ID 只能对应一个地区，切换地区需要先清空余额、取消所有订阅。
  - App 内订阅的退款、换套餐都要走苹果，不能在服务方网页上直接改。
- **费用参考**：社区实测 ChatGPT Plus 走这条路大约 ¥135–140/月（含礼品卡溢价）。
- **Google Play 礼品卡**：同理，但区锁更严格，账号地区、网络出口地区、付款资料三者要对得上。

#### 朋友代付

- **优点**：零成本，适合偶尔付一次。
- **缺点**：每月续费都要麻烦人家；账单和卡在别人名下，退款、发票、换套餐都要再找人；朋友换卡或卡过期，订阅就断。

#### 交易平台发行的联名卡

- **优点**：费率是所有卡类方案里最低的，普遍零月费。
- **缺点**：要先在发卡平台开户、做身份认证，并且先把钱换成平台支持的美元资产才能充值，链路长；不少平台对部分国家和地区不发卡，大陆可用性要自己确认。
- **适合**：本来就在用这类平台、熟悉操作的人。

#### 支持支付宝等国内方式入金的预付卡

- **优点**：入金方式最贴近国内用户习惯，不用另外开海外账户。
- **缺点**：这一类平台 2024–2025 年陆续有关停的，选之前看清楚运营时间、有没有退款渠道；最低充值额、能不能提现、身份认证要求各家差别很大。
- **怎么挑**：看费用是否在付款前全部列明、能否续充（卡号不变）、发卡是否自动、扣款失败收不收费、能不能联系到客服。

#### 一次性虚拟卡

- **优点**：用完即弃，不担心被重复扣款。
- **缺点**：订阅是按月扣的，一次性卡下个月已经失效，订阅会自动中断，每月都要重新买卡、重新绑卡。只适合付一次就结束的场景。

#### 第三方代充 / 合租账号

- **优点**：最简单，交钱就行。
- **缺点**：代充通常需要把账号密码交给对方；合租账号随时可能被改密码，也违反大多数 AI 服务的使用条款；聊天记录和文件对其他人可见。**不建议用于任何有工作资料的账号。**

---

## 4. Pink Card（利益相关）

> **利益相关：本仓库作者团队做 Pink Card。** 下面的内容是我们自己的产品介绍，请带着这个前提阅读，并和第 3 节其他方法对比后再决定。

**是什么**：预付虚拟卡，USD 计价，Mastercard / Visa 卡组织。先充值后消费，不是信用卡，没有授信。

**常用来付**：ChatGPT Plus、Cursor、Gemini、Google Cloud、Midjourney、OpenAI API 充值、部分海外网站订阅。Claude 付款前请先看第 6 节。

**怎么买**：官网 [pinkcard.cc](https://pinkcard.cc) 选面值下单，卡号、有效期、CVV 和可用的账单地址发到邮箱，然后去对应服务的网页端绑卡。网页面值 $110 起。付款方式以下单页为准，目前网站可用**支付宝扫码自动发卡（约 1–2 分钟）**（每笔订单单独生成收款码，按页面显示的人民币金额付款，另收 3% 通道费；手机上可直接拉起支付宝）或**网站账户余额**付款。支付宝付款成功后系统自动确认，一般 1–2 分钟内卡信息发到邮箱，不需要等客服核款；超过 10 分钟没收到，先看垃圾邮件箱，再带订单号联系客服。

**费用（全部列出）**：

| 项目 | 金额 |
|---|---|
| 开卡费 | $10 |
| 服务费 | 3%，按「面值 + 开卡费」计算 |
| 续充 | 每次 $5 + 充值金额的 5%，卡号不变，不用重新绑卡 |
| 支付宝付款 | 另加 3% 通道费 |
| 月费 | $2.50 / 月 |
| 交易费 | 每笔 $1，**扣款失败也收**；失败的每月最多收 3 笔 |

**算例**：买 $110 面值，需付 $110 + $10 + ($120 × 3%) = **$123.60**（用支付宝付再加 3%）。

**坦白说不便宜**：按月订一年 ChatGPT Plus（$240），在 Pink Card 上的附加成本大约 $61–74（开卡费、服务费、中途续充的 $5 + 5%、12 个月月费、12 笔交易费合计，不含支付宝 3%），约占订阅费的四分之一到三成。逐项算法见 [docs/fees.md](docs/fees.md)。第 3 节里零月费、费率 1% 左右的方案，同样场景下附加成本低得多。

**那为什么有人还选它**：

- 不用先去别的平台开户、换美元资产，下单就能拿到卡；
- 一张卡同时付 ChatGPT、Cursor、Gemini、Google Cloud 这类必须填卡号的订阅；
- 能续充，卡号不变，不用每月重新绑卡。

如果你只订一个服务、也不嫌多开一个平台账户麻烦，选零月费的方案更划算。

**用的时候注意**：

- 卡里常备 $25 左右（原因见第 5 节第 4 条），否则首笔容易因预授权失败，还会计一笔交易费；
- 账单地址照发卡邮件里给的填，网络出口地区选同一个国家；
- 不能用来充值 App Store / Google Play 礼品卡或内购，这两家按发卡行拦截，大部分虚拟卡都过不去；
- 卡号和 CVV 谁拿到谁能用，不要发到群里。

---

## 5. 付款被拒排障清单

> 关键词：Your card was declined 怎么办、card not supported、AVS 邮编不正确、续费失败。更细的报错对照见 [docs/card-declined.md](docs/card-declined.md)。

按顺序逐条排查，**每改一项再试一次，不要一口气连续重试**。

### 5.1 付款前检查

- [ ] **在网页端订阅**，不是在 App 里。App 内购走苹果 / 谷歌，和卡没关系，大部分虚拟卡也过不了这一道。
- [ ] **发卡行国家在服务范围内**。国内银行发的卡，不管是不是双币卡，基本都不行。
- [ ] **卡里余额 ≥ 标价 + 税 + 预授权余量**。$20 的订阅建议至少留 $25。
- [ ] **账单地址逐字段照抄**发卡方给的：街道、城市、州 / 省、邮编、国家要互相匹配。
- [ ] **网络出口地区**和账单地址在同一个国家，付款过程中不要切换。
- [ ] **浏览器自动填充关掉**，或者填完后人工核对一遍，自动填充经常把旧地址填进去。
- [ ] **同一张卡没有绑在多个账号上**。一卡多号是常见的风控信号。

### 5.2 按报错对照

| 你看到的提示 | 常见原因 | 怎么处理 |
|---|---|---|
| Your card was declined / 卡被拒绝 | 笼统拒绝，最常见是发卡行国家不支持，或商户风控 | 先确认卡的发卡国；是虚拟卡的话，核对账单地址和网络出口地区 |
| Your card does not support this type of purchase / card not supported | 卡段被商户拦截，常见于部分预付卡段 | 换一张卡段不同的卡，这种情况重试没有用 |
| Insufficient funds / 余额不足 | 余额没算上税和预授权 | 充到标价 + 至少 $5 再试 |
| Incorrect ZIP / 邮编不正确 / 地址校验失败 | AVS 不匹配 | 照发卡方给的地址逐字段重填，注意州和邮编对应 |
| Your card requires authentication / 3DS 验证失败 | 发卡行要求验证但没完成 | 留意发卡方的短信、邮件或 App 通知；页面别提前关 |
| Your payment could not be processed / 请稍后再试 | 短时间内失败次数太多，被临时风控 | **停下来**，至少隔几个小时；先在账户里删掉旧卡再重新绑 |
| 付款成功但很快被退款 / 订阅被取消 | 商户事后风控（地区、账号历史、付款方式不一致） | 别立刻换卡重试；先检查账号地区、登录地区是否一致 |

### 5.3 被拒之后的正确姿势

1. **不要连续重试。** 同一账号短时间内失败几次，风控会记住，之后换什么卡都更难过。很多预付卡失败也收手续费，连续重试还会白白扣钱。
2. **先删卡，再核对，再绑。** 在服务的付款设置里删除失败的卡，检查第 5.1 节每一项，间隔一段时间后重新绑卡。
3. **检查是不是被扣了预授权。** 失败的交易有时会先冻结一小笔，通常几天内自动释放，不是被扣走。
4. **一直不行就换方法**，不要在同一个账号上反复试同一类卡。

### 5.4 续费失败（第一个月成功，第二个月失败）

- 余额不够：自动续费那天卡里要有钱，记得提前续充；
- 一次性卡已经失效：换成能续充的卡；
- 卡过期或被冻结：看发卡方的通知邮件；
- 商户重试：余额不足时商户会在几天内反复重试，如果卡失败也收费，一定要尽快充值或取消订阅。


### 5.5 Claude Pro / ChatGPT Plus / Cursor 付款常见失败原因与排查

> 关键词：Claude Pro 付款失败、Claude 订阅 支付、ChatGPT Plus 付款被拒、ChatGPT Plus 国内 支付、Cursor 付款被拒、Cursor Pro 续费失败

三家网页端都通过 Stripe 收款，第 5.2 节的通用报错都适用。下面是各家**特有**的坑，按「最常见 → 少见」排列。

#### Claude Pro

| 现象 | 常见原因 | 排查 / 处理 |
|---|---|---|
| 订阅页直接打不开或提示地区不支持 | 账号使用地区不在 Anthropic 官方支持地区内 | 先查[官方支持地区列表](https://www.anthropic.com/supported-countries)；不在列表里的，付款成功也不代表能长期正常使用，先别付 |
| 卡被拒，换卡也被拒 | 短时间内多次失败触发风控；或卡的发卡国、账单地址、网络出口地区三者不一致 | 停止重试，至少隔几个小时；删掉失败的卡，核对账单地址逐字段与发卡方一致、网络出口地区与账单地址同一国家后再绑一次 |
| 付款成功，随后被退款或订阅被取消 | 事后风控：账号注册信息、登录地区、付款方式不一致 | 不要马上换卡再付；先确认账号资料和常用登录地区，必要时按官方帮助中心联系支持 |
| 要求上传证件 / 自拍做身份核验 | 官方隐私政策允许对部分用户做身份核验 | 付款前确认自己能满足官方核验要求 |
| App 内订阅失败 | App 内购走苹果 / 谷歌账单，和卡无关 | 改在网页端订阅；或用与 App Store 地区一致的付款方式 |

**客观风险提示**：Claude 对付款和账号的审核比其他几家严。付款成功不等于账号可以长期使用，账号能否持续使用取决于 Anthropic 的条款和审核，任何付款工具都无法保证。本指南不提供伪造地区或身份的方法。

#### ChatGPT Plus

| 现象 | 常见原因 | 排查 / 处理 |
|---|---|---|
| Your card was declined | 国内发卡行（含双币卡、全币种卡）的发卡国不在支持范围 | 换一张发卡国在服务范围内的卡；虚拟卡先核对账单地址 |
| 网页和 App 都显示没订上，但卡被扣了 | 预授权冻结，或网页 / App 两套账单重复 | 预授权一般几天内释放；先在「设置 → 订阅」确认是哪一套账单，别重复订 |
| 付款页一直转圈或提示请稍后再试 | 短时间内失败次数过多，被临时限制 | 停下来隔几个小时；换浏览器无痕窗口、关掉自动填充后再试 |
| 余额不足（明明够 $20） | 部分地区加税，加上预授权余量 | 卡里留 $25 以上 |
| 升级 Pro / Team 时被拒 | 金额大，余额或单笔限额不够 | 先按升级后的总价（含税）充够 |

#### Cursor

| 现象 | 常见原因 | 排查 / 处理 |
|---|---|---|
| 首次订阅 Pro 被拒 | 发卡国、卡段被拦截，或账单地址不匹配 | 同第 5.1 节；Cursor 只能网页付款，没有 App 内购可替代 |
| 订阅成功后月中又被扣款 / 扣款失败 | 开了按量计费（usage-based pricing），超出额度后单独扣款 | 在 Settings → Billing 里看是否开启按量计费、设好上限；卡里留出余量 |
| Teams 加人后扣款失败 | 新增席位会按比例补扣 | 加人前先确认余额够补扣金额 |
| 续费失败后功能被降级 | 自动续费当天余额不够或卡已失效 | 充值后在 Billing 页手动重试或更新卡；续充型的卡号不变，不用重新绑 |

#### 三家通用的排查顺序

1. 确认在**网页端**付款，不是 App 内购；
2. 确认卡的**发卡国**在服务范围内（国内银行卡基本不行）；
3. 余额 ≥ 标价 + 税 + 至少 $5 余量；
4. 账单地址逐字段照抄发卡方给的，关闭浏览器自动填充；
5. 网络出口地区和账单地址同一国家，付款过程中不要切换；
6. 失败一次就**停下来**，删卡、核对、隔一段时间再试，不要连续重试或连换多张卡。

---

## 6. Claude Pro 单独说明

> 关键词：Claude Pro 订阅付款、Claude 付款失败、Claude 支持地区

Claude 对付款和账号的审核比其他几家严，付款前多做几步确认：

> 2026 年 10 月初有报道称，部分香港地区的 Claude 账号（免费和 Pro 都有）被停用，Anthropic 未公布具体原因；用户和当地媒体归纳的可能因素包括数据中心 IP、虚拟卡或本地卡配海外账单地址、登录国家频繁变化（来源：VGTimes，2026-10-02）。另外，Anthropic 已更新隐私政策，可能要求部分用户上传政府签发的证件和自拍做身份核验（来源：TechCrunch，2026-06-22）。付款前先确认自己的账号情况能满足这些要求。

- 先看 Claude 官方的[「支持地区」列表](https://www.anthropic.com/supported-countries)，账号使用地区不在列表里的，先别付款；
- 账单地址、常用登录地区、账号资料尽量一致，不要频繁在多个地区之间切换；
- 付款被拒后不要连续换卡重试，先按第 5 节排查，等一段时间再试；
- 已经有 Pro 的：别频繁换卡或改账单地址，重要对话定期导出。

具体规则以 Claude 官方条款为准，社区传言变化很快，不要只看二手消息。

---

## 7. 怎么选：一张决策表

| 你的情况 | 建议 |
|---|---|
| 有海外实体卡或海外账户 | 直接用，最省心 |
| 只订 ChatGPT Plus、主要在 iPhone 上用 | 外区 Apple ID + 礼品卡可以考虑，注意礼品卡来源 |
| 已经在用交易平台、熟悉换汇操作 | 联名卡，费率最低 |
| 要同时付 ChatGPT、Cursor、Gemini、Google Cloud 等多个服务，不想多开平台账户 | 能续充的预付卡，比较各家费用后选 |
| 只付一次、不续费 | 一次性虚拟卡 |
| 要订 Claude Pro | 先看第 6 节的确认事项 |
| 账号里有工作资料 | 不要用代充或合租 |

---

## English Summary

**How to pay for ChatGPT Plus / Claude Pro / Gemini / Cursor / Midjourney when your local card gets declined — a comparison of methods and a decline-troubleshooting checklist (October 2026).**

- **Why cards fail**: merchants (mostly via Stripe; Gemini via Google Payments) check the card's issuing country (BIN), card type, billing address (AVS), network exit region, 3DS, and balance including tax and pre-authorization. Most "declined but I have money" cases come down to the issuing country.
- **Methods compared**: an overseas bank card in your own name (most reliable); a foreign-region Apple ID topped up with App Store gift cards (iOS in-app only, gift-card markup); a friend paying for you; cards issued by trading platforms (lowest fees, usually no monthly fee, but require an extra account, ID verification and converting funds to USD first); prepaid cards that accept local payment methods (convenient, but several providers shut down in 2024–2025, so check track record); single-use cards (break on renewal); resellers / shared accounts (not recommended).
- **Pink Card (disclosure: our team builds it)**: a prepaid USD Mastercard/Visa card. Fees: $10 issuance + 3% service fee (on face value + $10), $5 + 5% per top-up, $2.50/month, $1 per transaction including failed ones (failed ones capped at 3 per month); paying by Alipay adds 3%; Alipay payments on the website are confirmed automatically and the card is emailed in about 1–2 minutes. Web face value starts at $110. It is **not** the cheapest option: about $61–74 extra per year for a $20/month subscription. Its case is convenience: no extra platform account, one card for several subscriptions, reloadable with the same card number. Site: pinkcard.cc.
- **Decline checklist**: subscribe on the web, not in-app; keep at least $25 for a $20 plan; copy the billing address field by field; keep the network exit region in the same country as the billing address; turn off browser autofill; don't bind one card to several accounts; **don't retry repeatedly** — remove the card, fix the details, wait, then try again.
- **Claude Pro**: Claude reviews payments and accounts more strictly than others. Check the official supported-regions list first, keep billing address and login region consistent, and avoid retrying with many different cards.

- **More**: [English FAQ](docs/faq-en.md) · [fee comparison](docs/fees.md) · [changelog](CHANGELOG.md)

---

## 延伸阅读：分篇 FAQ

| 文章 | 适合谁 |
|---|---|
| [各 AI 服务付款步骤](docs/payment-steps.md) | 第一次订阅 ChatGPT Plus / Claude Pro / Cursor / Gemini / Midjourney |
| [Claude Pro / ChatGPT Plus / Cursor 付款失败排查](docs/claude-chatgpt-cursor-payment-failed.md) | 三家各自特有的付款失败原因 |
| [常见拒付原因与解决](docs/card-declined.md) | 已经看到「Your card was declined」或续费失败 |
| [费用对比表](docs/fees.md) | 想算清一年下来各种方法多花多少钱 |
| [English FAQ](docs/faq-en.md) | Non-Chinese readers |

---

*本仓库内容仅供参考，不构成任何金融建议。各服务的条款和费用以官方页面为准。*
