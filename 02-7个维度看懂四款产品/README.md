# 02 · 7 个维度看懂主流 PersonalAgent

> 最后验证：2026-10-09 ｜ 阅读时间：10 分钟 ｜ 国内可用性：待作者实测

先认识五款主流产品，再用 7 个问题把它们放在一起比，最后按你要做的事挑一款。

---

## 第一部分：五款产品，各一张名片

### 🟠 Grok Bot · 一支会自己扩编的数字员工队伍

- **出自**：SpaceXAI / xAI，架在 Cursor 的基础设施上[^aibot]
- **最大特点**：可以开很多个 Bot，按角色分工，在群聊里协作，Bot 还能再创建 Bot[^aibot][^aim]
- **怎么干活**：不需要 API，直接在网页界面上像真人一样点击、填写[^aibot]
- **价格**：约 $20/月起，随 Cursor 或 SuperGrok 订阅附带[^aim]
- **要注意**：同一个账号下的所有 Bot 共用一台电脑和全部登录，Bot 之间**不是权限边界**[^cp]
- **适合**：想给公司、团队配"数字员工"的人

### 🔵 Muse · 一个越来越懂你的私人管家

- **出自**：Meta[^meta]
- **最大特点**：一个主 Agent 长期跟着你，记忆以可编辑的文本保存[^aim]
- **怎么用**：Muse App、网页，或者直接在 WhatsApp 里聊[^wiki]
- **价格**：有免费档；Power $20/月、Maximum $100/月[^aim]
- **要注意**：目前只在美国、加拿大可用；默认会用你的数据训练模型，可以关闭[^wiki][^cp]
- **适合**：个人和家庭事务

### 🟢 Cue · 有自己电话、邮箱和钱包的办事员

- **出自**：Manus（团队起家于中国，现总部在新加坡）[^bbg]
- **最大特点**：每个 Agent 都有独立的邮箱、电话号码和钱包，能替你打电话、在预算内付款[^tnw]
- **价格**：内测期免费，需要邀请码[^cp]
- **要注意**：安全设计、数据存放地公开得很少；国内版在准备中[^cp]
- **适合**：需要 Agent 替你对外联系的事

### ⚫ Dots · 住在 ChatGPT 里的常驻助理

- **出自**：OpenAI[^tc]
- **最大特点**：通过插件连接 4000 多个应用，能在 Slack、Teams 里找它[^tc]
- **价格**：随 ChatGPT Pro 附带，约 $100/月起[^aim]
- **要注意**：记忆不能单条修改，只能整体重置[^aim]；Pro 不包含欧洲经济区、英国、瑞士[^cp]
- **适合**：已经离不开 ChatGPT 的人和团队

### 🟣 Instinct · 发条短信就能使唤的私人助理

- **出自**：Spear Street Technology，旧金山的创业公司，创始人 Noah Shinn 曾是 Sierra 的研究科学家[^vellum]
- **最大特点**：没有 App。直接发短信、打电话，或者通过 iMessage、WhatsApp 找它；它也会主动打电话给你[^every]
- **常用来做**：订行程、谈账单、跟进邮件、排日程；据报道，它做的事里超过一半是订行程[^vellum]
- **价格**：邀请制内测，内测期免费，正式价格未公布[^every]
- **要注意**：要接入邮箱、消息、屏幕、音频和位置，权限是五款里最多的[^vellum]；安全公司报告撤销授权后数据仍被保留[^noma]；不少信息来自第三方上手测试，确定性较低[^every]
- **适合**：个人杂事多、愿意多交一些权限来换省心的人

> ⚠️ 价格各来源说法不完全一致，请以官网为准。

---

## 第二部分：用 7 个问题比一比

这 7 个问题适用于任何 Agent，不止这五款。以后看到新产品，拿它们问一遍就行。

> 7 个维度是本书作者的原创框架；表中每一格的判断都有出处，见文末。

| 问题 | Grok Bot | Muse | Cue | Dots | Instinct |
|---|:---:|:---:|:---:|:---:|:---:|
| **① 执行力**：能真的帮我操作网站和软件吗？ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **② 持续性**：我关掉 App，它还在干活吗？ | ✅ 最强 | ✅ | ⚠️ | ✅ | ✅ 最主动 |
| **③ 身份**：用我的账号，还是有它自己的？ | ❌ | ⚠️ | ✅ 最强 | ❌ | ⚠️ |
| **④ 可控性**：花钱、发消息前会先问我吗？ | ⚠️ | ✅ 最透明 | ⚠️ | ✅ | ⚠️ |
| **⑤ 记忆**：记得住我吗？我能改吗？ | ❓ | ✅ | ❓ | ⚠️ | ⚠️ |
| **⑥ 协作**：能开好几个一起干吗？ | ✅ 最强 | ⚠️ | ✅ | ❌ | ❌ |
| **⑦ 隐私**：我的数据去哪了？ | ⚠️ | ⚠️ | ❓ | ⚠️ | ❌ 风险最大 |

✅ 有且较强　⚠️ 有但有限制　❌ 没有　❓ 未公开

### 每一格为什么这么打分

<details>
<summary><b>① 执行力</b>：五款都有自己的电脑</summary>

- Grok Bot：云端虚拟机；不需要 API，直接操作网页界面[^cp][^aibot]
- Muse：每个用户一台独立的虚拟机；Mac 版可以操作本地应用[^cp][^wiki]
- Cue：每个 Agent 一台电脑，隔离方式未公开[^cp]
- Dots：每个 dot 一台云电脑，还可以连接一台你自己的电脑[^cp]
- Instinct：云端电脑，还能打电话（来自上手测试）[^every]
</details>

<details>
<summary><b>② 持续性</b>：Grok Bot 触发方式最多，Instinct 最主动</summary>

- Grok Bot：可以按定时、webhook、PR、CI 失败、Slack 消息自动启动[^cp]
- Muse：你关掉 App 后会继续干活[^wiki]
- Cue：没有公开的定时或触发功能[^cp]
- Dots：后台运行，支持定时检查[^cp][^tc]
- Instinct：会主动给你发短信、打电话；有报道称可由邮件和日历触发[^every]
</details>

<details>
<summary><b>③ 身份</b>：只有 Cue 给了 Agent 独立身份</summary>

- Grok Bot：用你的登录，同一账号的所有 Bot 共用[^cp]
- Muse：用你连接的账号，但它看不到真实密码和卡号[^cp]；它有自己的邮箱地址[^wiki]
- Cue：每个 Agent 有独立的邮箱、电话、钱包[^cp][^tnw]
- Dots：只有 ChatGPT 里的身份，没有电话、邮箱、钱包[^cp]
- Instinct：能打电话；自己的邮箱正在推出，发消息时用什么身份还不清楚[^every]

**为什么重要**：Agent 用的是自己的身份时，出了事你能算清楚损失在哪里；用你的身份时，它能动的就是你的全部。
</details>

<details>
<summary><b>④ 可控性</b>：Muse 公开得最详细</summary>

- Grok Bot：有企业级治理（成员管理、审计日志），但没有设置策略时，网络访问默认全部放行[^cp]
- Muse：有专门拦截危险操作的机制，敏感操作要你确认，付款用一次性卡号[^cp][^da]
- Cue：只公开了预算上限和"最后由你决定"[^cp][^da]
- Dots：可以设四级的自定义规则，有自动审查和只读模式[^cp][^da]
- Instinct：发消息和付款前会先问你，但只在一次上手测试中观察到[^every]；安全公司报告过它不经确认就执行操作[^noma]
</details>

<details>
<summary><b>⑤ 记忆</b>：只有 Muse 能让你直接改</summary>

- Grok Bot：文档没说明，也没有查看或编辑记忆的方法[^aim]
- Muse：记忆以可编辑的文本文件保存[^aim]
- Cue：未公开
- Dots：会从反馈中学习偏好，但不能单条修改，只能整体重置[^aim]
- Instinct：能跨对话记住，但召回不稳定；可以删除数据，没有直接编辑的方法[^every]
</details>

<details>
<summary><b>⑥ 协作</b>：Grok Bot 和 Cue 能组队</summary>

- Grok Bot：约 50 个按角色分工的 Bot，可以在群聊里协作[^aim][^cp]
- Muse：一个主 Agent，加上子对话和子 Agent[^cp]
- Cue：多个 Agent 在群聊里交接工作[^cp]
- Dots：目前只有一个，组队还只是规划[^cp]
- Instinct：只有一个[^every]
</details>

<details>
<summary><b>⑦ 隐私</b>：没有一款能打满分，Instinct 风险最大</summary>

- Grok Bot：数据只托管在美国[^cp]
- Muse：默认用你的数据训练模型，可以关闭；之后会推出只有你持有密钥的加密虚拟机[^meta][^cp]
- Cue：训练用途、数据存放地都未公开[^cp]
- Dots：隔离方式、数据存放地区未公开[^cp]
- Instinct：数据授权范围很宽；撤销授权后数据仍被保留[^noma]；可以选择不让它用你的数据训练模型，但有安全审查的例外[^every]

**为什么重要**：越主动的 Agent，需要的权限越多。Instinct 的"省心"，是用最多的权限换来的。
</details>

---

## 第三部分：按你要做的事挑一款

没有"最好的 Agent"，只有"最适合这件事的 Agent"。

### 第一步：先过四道关

在比较好坏之前，先确认你**用得上**。按顺序问自己[^da]：

1. 🔑 我的账号能访问这个产品吗？（在国内，先看[第四部分](#第四部分国内能用吗)）
2. 🔌 它能接上这件事需要的数据和应用吗？
3. 🛡️ 它的安全管控，够这件事用吗？
4. 🧪 先拿一件无害的小事试一试，它守得住边界吗？

四关都过了，再往下看。

### 第二步：这件事适合交给 Agent 吗？

一篇广为流传的 X 帖子给了五个标准[^rafy]。一件事越符合，越适合交出去：

- ✅ **可重复**：不是一次性的
- ✅ **跨系统**：要在好几个工具之间来回搬
- ✅ **有规则可循**：说得清怎样才算做对
- ✅ **先出草稿**：Agent 交初稿，你来拍板
- ✅ **错了能挽回**：出错的代价有限

> 该帖自称内容引自官方资料，原件尚未找到，仅作参考。

### 第三步：按场景挑产品

| 你想让它… | 首选 | 为什么 |
|---|---|---|
| 在好几个网站之间重复操作（填表、搬数据） | **Grok Bot** | 不需要 API，直接操作网页界面，能录制成工作流[^aibot] |
| 同时处理一大批任务 | **Grok Bot** | 可以开很多个 Bot 并行[^aim] |
| 公司里某件事一发生就自动处理 | **Grok Bot** | 支持定时、webhook、Slack 消息等多种触发[^cp] |
| 替你打电话、预约、对外联系 | **Cue** | 每个 Agent 有自己的电话和邮箱[^tnw] |
| 在一笔预算内替你花钱 | **Cue** / **Muse** | Cue 有钱包和预算上限[^tnw]；Muse 用一次性卡号付款[^cp] |
| 网购、订行程（在美国或加拿大） | **Muse** | 接入了很多电商和出行平台[^wiki] |
| 在 Slack、Teams 和各种办公软件里干活 | **Dots** | 能连接 4000 多个应用[^tc] |
| 不想装 App，发条短信就让它办事 | **Instinct** | 短信、电话、iMessage、WhatsApp 都能用，还会主动打给你[^every] |
| 订行程、谈账单、各种生活杂事 | **Instinct** / **Muse** | Instinct 一半以上的活是订行程[^vellum]；Muse 接入了电商和出行平台[^wiki] |
| 先免费试试 | **Muse** 免费档 / **Cue**、**Instinct** 内测 | 门槛最低[^aim][^cp][^every] |

### 一张图帮你选

```
你在中国大陆吗？
├─ 是 → 先看本章第四部分「国内能用吗？」（待作者实测）
└─ 否 ↓

你想让它做什么？
├─ 个人和家庭的日常事务 ──────→ Muse
├─ 生活杂事，愿意多交权限 ────→ Instinct（邀请制）
├─ 替我对外打电话、联系人 ────→ Cue
├─ 我已经整天在用 ChatGPT ───→ Dots
└─ 给公司、团队配数字员工 ────→ Grok Bot
```

横评的结论也大体如此：要独立对外身份选 Cue，要清楚的审批边界选 Muse，已经在用 ChatGPT 选 Dots，按角色分工做公司工作选 Grok Bot[^cp]。另一份榜单把 Instinct 评为"最能干、最主动"[^top5]。

### 本书为什么主要用 Grok Bot 举例

本书的场景手册面向 CEO 和创始人。他们要的是给公司搭一支数字员工团队，这正是 Grok Bot 在多份横评里都被认可的长处：持续运行、按角色分工、多 Bot 协作[^cp][^aim]。

但它也有明显的短板：所有 Bot 共用你的登录、没设策略时网络访问默认全放行、数据只托管在美国[^cp]。用之前请对照上面的第二部分。

> 作者目前与文中任何产品都没有合作。广告位待租 😄

---

## 第四部分：国内能用吗？

**目前没有可靠的结论。**

- 英文横评 CodePick 的判断是"Grok Bot、Muse、Cue、Dots 四款在中国大陆都还用不了"[^cp]
- Instinct 靠短信和电话使用，在国内能否使用，目前没有找到资料
- 网上也有"Grok Bot 国内可以直连"的文章[^163]，但那是作者自己的使用体验，官方没有确认

本书会在作者实测后更新这一节，并写明测试日期、网络环境和账号所在地区。

> 🚫 网上有代充、"镜像站"的推广，请谨慎。镜像站提供的通常只是 Grok 聊天模型，不是 Grok Bot。

---

**下一章**：03 · 场景手册，CEO 和职场执行层，分两条路线把 Agent 真正用起来（即将上线）。

## 参考来源

访问日期均为 2026-10-08（Instinct 相关为 2026-10-09）。

[^aim]: AIMultiple,《Always-On Agents: Dots vs Grok Bot vs Muse》, https://aimultiple.com/always-on-agents
[^cp]: CodePick,《Cue vs Muse vs Grok Bot vs Dots (2026): Four Persistent Agents》, https://codepick.dev/en/compare/cue-vs-muse-vs-grok-bot-vs-dots-2026/
[^da]: Digital Applied,《Personal AI Agents Compared: Dots, Muse, Cue and Grok》, https://www.digitalapplied.com/blog/personal-ai-agents-compared-dots-muse-manus
[^aibot]: AI 工具集,《Grok Bot - SpaceXAI 推出的 AI Agent 系统》, https://ai-bot.cn/grok-bot/
[^wiki]: Wikipedia,《Muse (AI agent)》, https://en.wikipedia.org/wiki/Muse_(AI_agent)
[^meta]: Meta,《Introducing Muse》, 2026-09, https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/
[^bbg]: Bloomberg,《Manus Expands AI Agent Tools With New Multipurpose Model, Cue App》, 2026-09-28, https://www.bloomberg.com/news/articles/2026-09-28/manus-expands-ai-tools-in-renewed-push-into-agent-market
[^tnw]: The Next Web,《Manus 2.0 and Cue give AI agents their own email, phone and wallet》, https://thenextweb.com/news/manus-2-0-cue-ai-agents-email-phone-wallet
[^tc]: TechCrunch,《OpenAI launches Dots, its bubbly agentic avatar》, 2026-09-29, https://techcrunch.com/2026/09/29/openai-launches-dots-its-bubbly-agentic-avatar/
[^rafy]: @0xRafy, X, 2026-09-22, https://x.com/0xRafy/status/2102149561867292887 ｜作者身份未知｜内容来源未核实
[^every]: Every,《Dot vs. Gemini Spark vs. Grok Bot vs. Hermes Agent vs. Instinct vs. Muse vs. OpenClaw vs. Poke》, https://every.to/personal-agents-comparison
[^vellum]: Vellum,《Official Instinct Breakdown (2026)》, https://www.vellum.ai/blog/official-instinct-breakdown ｜Vellum 做同类产品（利益相关）
[^noma]: Noma Security,《Personal AI Agent Security: Discovering and Governing dots, Grok Bot, Instinct, Muse, & Muse Code》, https://noma.security/blog/personal-ai-agent-security-discovering-and-governing-dots-grok-bot-muse-muse-code ｜Noma 做 AI 安全产品（利益相关）
[^top5]: Top5Apps,《Best Personal AI Agents: 5 Worth Trying [Reviewed Oct 2026]》, https://top5apps.ai/best-ai-apps/best-personal-ai-agents/
[^163]: 网易号,《Grok Bot 国内直接订阅教程》, https://www.163.com/dy/article/L5RTFEP5055625DH.html
