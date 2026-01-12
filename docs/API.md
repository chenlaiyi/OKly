# OKly API 文档

## 基础信息

- **API Base URL**: `https://ly.ddg.org.cn/api`
- **WebSocket URL**: `wss://ly.ddg.org.cn`
- **认证方式**: API Key (Header: `Authorization`)

## 接口列表

### 1. 行情相关

#### 获取市场行情
\`\`\`
GET /markets
\`\`\`

**响应示例**:
\`\`\`json
{
  "success": true,
  "data": [
    {
      "inst_id": "BTC-USDT-SWAP",
      "last": "95000.5",
      "open24h": "95200.0",
      "volume": "1234567",
      "high24h": "96000.0",
      "low24h": "94000.0"
    }
  ]
}
\`\`\`

#### 获取K线数据
\`\`\`
GET /candles?symbol={symbol}&limit={limit}
\`\`\`

**参数**:
- `symbol`: 交易对ID (如 BTC-USDT-SWAP)
- `limit`: 数据条数 (默认100)

### 2. 交易相关

#### 执行交易
\`\`\`
POST /trade
Content-Type: application/json

{
  "symbol": "BTC-USDT-SWAP",
  "side": "long",
  "size": 1
}
\`\`\`

#### 平仓
\`\`\`
POST /positions/close
Content-Type: application/json

{
  "positionId": "uuid"
}
\`\`\`

### 3. AI分析

#### 获取最新AI分析
\`\`\`
GET /ai/analysis/latest?symbol={symbol}
\`\`\`

### 4. 策略管理

#### 获取策略列表
\`\`\`
GET /strategy
\`\`\`

#### 创建策略
\`\`\`
POST /strategy
Content-Type: application/json

{
  "name": "我的策略",
  "description": "策略描述",
  "fund_config": {...},
  "buy_strategy": {...},
  "sell_strategy": {...},
  "risk_control": {...}
}
\`\`\`

更多接口请参考各端的API服务封装代码。
