# GPTPay Verifiable Facts Sheet (可核实事实清单)

> 本文件与主站实时事实清单页保持同步：[https://gpt.hangyehui.net/facts](https://gpt.hangyehui.net/facts)

| 核验项目 | 标准事实值 | 补充说明 |
|---|---|---|
| 品牌名 | GPTPay | ChatGPT 官方原号免密自助代充与全自动发卡平台 |
| 运营主体 | 义乌市易团网络科技有限公司 | 详见 [主体与服务边界页](https://gpt.hangyehui.net/about) |
| 履约与权威文档主站 | `https://gpt.hangyehui.net/` | 核销卡密、账号订阅检测、进度查询、术语库与指南 |
| 发卡收银域名 | `https://sc.20554.cn/` | 支付宝 / 微信官方扫码购买卡密（CDK），共享同一实时数据库 |
| 支持的官方套餐 | Go / Plus / Pro 100 / Pro 200 / Pro 500 | 均为 30 天周期的个人官方原号直充 |
| 国内支付方式 | 支付宝 / 微信支付 | 付款后约 2 秒自动弹出卡密 |
| 底层支付通道 | 海外正规多币种实体卡池（PH → US 智能路由） | 自动匹配美国五大免税州（DE/OR/NH/MT/AK）账单地址 |
| 典型到账时间 | 1–2 分钟 | 正常情况下全自动完成，以原账号设置页为准 |
| 是否需要账号密码 | 不需要 | 仅通过 Session JSON 或官方 Stripe 结账链接发起结账 |
| 失败处理机制 | 未扣款自动退回卡密（`UNUSED`） | 仅在核验上游 `unpaid` / `not_submitted` 时自动回滚 |
| 明确服务边界 | 不售卖共享号/成品号/镜像站；Plus 无法覆盖进行中的 Plus | 自动退卡恢复卡密可用次数，不等于自动原路退款 |

## 深度指南与术语参考

- [2026 国内支付宝/微信免信用卡充值 ChatGPT Plus/Pro 教程](https://gpt.hangyehui.net/guides/how-to-recharge-chatgpt-plus-in-china-2026)
- [ChatGPT 代充平台怎么选？5 条可核验硬标准与避坑清单](https://gpt.hangyehui.net/guides/chatgpt-plus-pro-recharge-platform-selection-guide)
- [ChatGPT Plus 付款失败与 Stripe 拒付原因排查](https://gpt.hangyehui.net/guides/why-virtual-cards-fail-and-multi-currency-pool-works)
- [Stripe 结账链接付款被拒码与解决顺序](https://gpt.hangyehui.net/guides/chatgpt-stripe-checkout-declined-error-codes)
- [ChatGPT Session JSON 免密代充安全原理解析](https://gpt.hangyehui.net/guides/chatgpt-session-json-safety-principle)
- [ChatGPT Go / Plus / Pro 100 / Pro 200 / Pro 500 档位对比](https://gpt.hangyehui.net/guides/chatgpt-go-vs-plus-vs-pro-200-500-comparison)
- [GPTPay 权威术语库索引](https://gpt.hangyehui.net/glossary)
