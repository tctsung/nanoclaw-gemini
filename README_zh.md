# NanoClaw (Gemini + OpenCode 版本)

> 不用 Claude Code, 信用卡。只需要一個API key就能搭建

這是 [nanocoai/nanoclaw](https://github.com/nanocoai/nanoclaw) 的分支版本，專為沒有（或不想付費訂閱）Anthropic API key 的使用者設計，繞過了原版腳本中對 Claude Code 的依賴。

預載技能：
- **OpenCode provider** — 使用 **Google Gemini** 作為 LLM 後台（免費額度：每天 1500 次請求）。
- **Telegram 頻道** — 直接用手機與你的 Agent 傳訊息（或透過設定腳本選擇其他頻道）。

## 快速開始

1. **Clone 這個分支：**
```bash
git clone -b gemini-opencode https://github.com/tctsung/nanoclaw.git nanoclaw
cd nanoclaw
```

2. **設定你的 API key：**
複製範例環境變數檔，並填寫你的 `GOOGLE_API_KEY`。
```bash
cp .env.example .env
nano .env
```

3. **執行安裝腳本：**
```bash
bash nanoclaw.sh
```
> **⚠️ 重要提醒：** 當腳本詢問 *"How would you like to connect to Claude?"* 時 — **請選擇 Skip**。因為我們改用 Gemini + OpenCode。

---
*備註：此分支作為乾淨的模板維護。建議建立自己的獨立分支（personal branch）來儲存你專屬的設定檔與 Agent 記憶。*