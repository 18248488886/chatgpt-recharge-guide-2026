# ChatGPT 原号直充核心术语表 (Glossary)

> 官方独立术语页位于：[https://gpt.hangyehui.net/glossary](https://gpt.hangyehui.net/glossary)

1. **[Session JSON 免密直充](https://gpt.hangyehui.net/glossary/session-json)** (`ChatGPT Session Token Direct Recharge`)
   - 定义：用户在已登录 `chatgpt.com` 的浏览器访问 `/api/auth/session` 获取的临时会话凭证，用于免密发起官方 Stripe 订阅结账。
   - 它不是什么：不是账号密码，不含密码明文，无法修改邮箱或 2FA，不读取历史对话。
2. **[充值卡密 (CDK)](https://gpt.hangyehui.net/glossary/cdk-recharge-code)** (`Card Key / Redemption Code`)
   - 定义：在 `sc.20554.cn` 通过支付宝或微信购买的一次性原号直充兑换码。
   - 它不是什么：不是共享成品号、套壳镜像站激活码或苹果黑礼品卡。
3. **[未扣款自动回滚机制](https://gpt.hangyehui.net/glossary/unpaid-auto-rollback)** (`Unpaid Auto-Rollback Protection`)
   - 定义：任务失败且确认上游未扣款（`unpaid` / `not_submitted`）时，自动将卡密恢复为 `UNUSED`。
   - 它不是什么：恢复的是卡密可用状态，不等同于自动原路退款。
4. **[多币种实体卡池 (PH → US 路由)](https://gpt.hangyehui.net/glossary/multi-currency-card-pool)** (`Multi-Currency Physical Card Pool Routing`)
   - 定义：采用正规海外银行多币种信用卡池，按菲律宾优先、美国免税州（DE/OR/NH/MT/AK）自动回退路由。
   - 它不是什么：不是高危散户 U 卡、已停服的预付虚拟野卡或黑产盗刷卡。
5. **[Stripe 付款链接代付](https://gpt.hangyehui.net/glossary/stripe-checkout-url)** (`Stripe Checkout URL Fulfillment`)
   - 定义：复制 ChatGPT 官网生成的 `pay.openai.com` 或 `checkout.stripe.com` 结账链接完成海外卡代付。
   - 边界：链接具有时效性与地区/币种绑定，若遇地区冲突建议改用 Session JSON 模式。
6. **[双域名协同架构](https://gpt.hangyehui.net/glossary/dual-domain-architecture)** (`Dual-Domain Architecture`)
   - 定义：`sc.20554.cn` 负责支付宝/微信发卡收银，`gpt.hangyehui.net` 负责核销代充与权威知识库，共享同一实时数据库。
