Position
- holding of asset, in point-of-time
- aka. 持仓，头寸（于外汇，利率，衍生品交易场景）

# Data
(Daily) Trade Blotter
- (每日)交易記錄manifest



# Actions
square trade
- aka. square off trades, 平仓

Rollover
- aka. 展期
- Used in FX Forward, Fixed Deposit

Straight-Through Processing (STP)
- 前中後台的整合：交易從前台到後台的自動化流程


## Repo
所有 repo 的核心机制是：以证券作为抵押，换取现金

Repo / Reverse Repo 交易類型
- aka. 回購或逆回購交易


### collateral
haircut
- aka. 折讓
- 資產估值時所施加的折扣。
  - `Collateral Value = Notional Value(名義價值) × (1−Haircut)`

Collateral mgmt
- Allocation: 挑选最合适的资产用于抵押
  - reuse: 重复使用抵押品（如再质押）
  - Substitution: 更便宜但合规的资产替换当前抵押品, 避免使用高成本资产
  - Liquidity Limit: 保证抵押品使用后仍能维持足够的流动性
- Compliance: Basel III, EMIR, Dodd-Frank
- Margin Call
  - 当交易对手的风险敞口超过约定的抵押品覆盖范围时，风控发出通知，要求对手补充抵押品。
  - 触发场景
    - 市场波动导致资产价值下降
      - 衍生品合约的市值变动 MTM 
    - 合约中设定的 Threshold 被突破
      - 抵押品价值低于最低保证金门槛（Minimum Transfer Amount）
