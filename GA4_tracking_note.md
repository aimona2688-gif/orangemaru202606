# GA4 追蹤筆記

## 事件名稱
- `add_to_cart`

## 目前埋設位置
- 檔案：[index.html](index.html)
- 按鈕位置：產品區塊的「加入購物車」按鈕
- 觸發方式：點擊按鈕時呼叫 `gtag("event", "add_to_cart", payload)`

## 事件 payload
- `currency: "TWD"`
- `value: 1234`
- `coupon: "SUMMER_FUN"`
- `shipping_tier: "Ground"`
- `items`：包含商品資訊

## 已確認事項
- 本地程式碼已正確加入 GA4 `add_to_cart` 事件
- 事件名稱使用底線格式 `add_to_cart`
- 需在正式公開頁面（GitHub Pages）重新整理後再到 GA4 即時報表驗證

## 備註
- 若 GA4 報表中仍沒有出現，請先確認：
  1. 公開網址已重新部署
  2. 使用公開網址測試，而不是本地 `file://` 頁面
  3. GA4 即時報表等待 1–5 分鐘後再確認
