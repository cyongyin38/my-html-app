# JUE SPACE · 身心靈療癒 APP 起始專案

這份專案包含兩個子專案,你需要把它們**分別跑起來**:

```
jue-space/
├── jue-space-api/      ← 後端 API(放在 Vercel 上,連 Neon 資料庫)
└── jue-space-app/      ← 手機 APP(用 Expo 寫,可同時打包 iOS / Android)
```

---

## 你要先裝這幾個東西(在你的 Windows 筆電上)

### 1. Node.js(讓你電腦能跑 JavaScript)
- 到 https://nodejs.org 下載 **LTS 版本**(20.x 或 22.x)
- 一路 Next 安裝
- 安裝完打開 PowerShell,輸入 `node -v`,有看到版本號就成功

### 2. Git(管理程式碼版本)
- 到 https://git-scm.com/download/win 下載安裝
- 安裝完打開 PowerShell,輸入 `git --version`,有看到版本號就成功

### 3. Cursor(AI 程式編輯器)
- 到 https://cursor.com 下載
- 用 Google 帳號登入

### 4. Expo Go(在你手機上)
- iPhone:App Store 搜「Expo Go」下載
- Android:Google Play 搜「Expo Go」下載
- 這是讓你**不用上架就能在手機上看 APP 的工具**,改一行程式手機立刻看到變化

---

## 起步順序(認真照順序走,不要跳)

### Step 1:先讓後端 API 跑起來(約 30-60 分鐘)
打開 `jue-space-api/` 資料夾的 `README.md`,跟著做。

### Step 2:再讓手機 APP 跑起來(約 30-60 分鐘)
打開 `jue-space-app/` 資料夾的 `README.md`,跟著做。

### Step 3:用手機掃 QR Code,你的 APP 就在手機上跑了!

---

## 你會用到的服務(全部都有免費方案)

| 服務 | 用途 | 你要做什麼 |
|---|---|---|
| **Neon** (你已有) | PostgreSQL 資料庫 | 拿到「連線字串」 |
| **Vercel** (你已有) | 跑後端 API | 連 GitHub 自動部署 |
| **Clerk** | 會員登入(含 Google/Apple/FB 登入) | 註冊免費帳號,拿金鑰 |
| **Stripe** | 國際金流(信用卡、Apple Pay、Google Pay) | 註冊,先用測試模式 |
| **Mux** | 課程影片串流 | 之後加課程影片時再申請 |
| **綠界** (你已有) | 台灣金流 | 已有,完成商店申請即可 |

---

## 接下來怎麼用 AI 把功能長出來?

當你跑通第一版後,任何你想加的功能(例如「加塔羅功能」、「加打卡功能」),你都這樣做:

1. 打開 Cursor
2. 按 `Ctrl + L` 開啟 AI 對話
3. 把這份 README 拖進對話框當參考
4. 跟它說:**「在 jue-space-app 加一個塔羅抽牌功能,有 22 張大牌,點下去翻面顯示牌義。樣式照現有 theme.ts 的顏色。」**

AI 會直接幫你改檔案。你按「接受」就好了。

---

## 卡關時的 SOS 三步驟

1. **錯誤訊息整段複製**(紅字、黃字都複製)
2. **貼給 Claude**(在 https://claude.ai)
3. 問:「我在做 JUE SPACE 專案,跑到 [某步驟] 出現這個錯誤,我用 Windows + Node.js 20,怎麼解?」

90% 的問題都能這樣解掉。

---

## 顏色設定(你的品牌色)

兩個專案都已經把你的品牌色設定在 `theme.ts` 裡了:

```
淡藕色 #D9B8B0(主要)
米白色 #FAF6F2(背景)
淺棕色 #A88A66(強調)
```

之後 AI 寫新元件時會自動沿用這套色票。如果想微調,只改 `theme.ts` 一個檔案,整個 APP 就跟著變。

---

**起步順序,再說一次:`jue-space-api/README.md` → `jue-space-app/README.md`**

Good luck 🌿
