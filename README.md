# bot-monitor
LINE Bot 監控 https://achir1015.github.io/bot-monitor/
<img width="1270" height="714" alt="image" src="https://github.com/user-attachments/assets/0297ad2c-8434-473c-9e02-175e73832390" />
這是完整的 HTML 監控儀表板，下載後直接用瀏覽器開啟即可。
功能說明：
▶ Verify 按鈕邏輯（三段式偵測）

先送 POST 請求，如果有回應（含 4xx）→ 顯示 ✔ 端點可達 + HTTP 狀態碼 + 耗時
若 CORS 擋住 → 改用 no-cors 模式再試，確認網路可達
若 8 秒內無回應 → 顯示「連線逾時，確認 ngrok 是否執行」

✦ 全部驗證 按鈕會同時觸發所有機器人驗證。
＋ 新增機器人 卡片（虛線框）→ 填入名稱、Channel、URL、Emoji 即可擴充，不需改程式碼。
