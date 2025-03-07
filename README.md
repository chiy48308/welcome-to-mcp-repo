# Cursor MCP 使用指南

[前面的內容保持不變...]

## 具體使用示例：創建和管理一個新項目

以下是一個完整的工作流程示例，展示如何使用 Cursor MCP 創建和管理一個新的 Web 應用項目：

### 1. 項目初始化

```bash
# 創建新的倉庫
建立一個名為 "my-web-app" 的新倉庫
自動初始化包含 README.md

# 克隆倉庫到本地
git clone https://github.com/您的用戶名/my-web-app.git
cd my-web-app
```

### 2. 設置項目結構

```plaintext
my-web-app/
├── src/
│   ├── components/
│   ├── pages/
│   └── utils/
├── public/
├── tests/
├── package.json
└── README.md
```

### 3. 功能開發流程

```bash
# 創建新的功能分支
建立名為 "feature/user-auth" 的新分支

# 添加新文件
創建 src/components/Login.js
更新 README.md 添加項目說明

# 提交更改
git add .
git commit -m "添加用戶登錄組件"
git push origin feature/user-auth
```

### 4. 問題追蹤和協作

```bash
# 創建新的問題（Issue）
標題：實現用戶認證功能
描述：
- 添加登錄表單
- 實現 JWT 認證
- 添加用戶資料頁面

# 創建拉取請求（Pull Request）
從 feature/user-auth 分支到 main 分支
添加代碼審查者
```

### 5. 代碼審查和合併

```bash
# 審查評論示例
在 Pull Request 中添加評論：
"請添加輸入驗證邏輯"

# 處理反饋
更新代碼
提交新的更改
請求重新審查
```

### 6. 發布和部署

```bash
# 合併到主分支
合併 Pull Request
刪除功能分支

# 創建發布標籤
git tag -a v1.0.0 -m "首次發布"
git push origin v1.0.0
```

### 7. 項目維護

```bash
# 處理問題報告
創建新的問題來追蹤 bug
分配給團隊成員
設置優先級和標籤

# 更新文檔
更新 README.md
添加新的文檔頁面
```

### 實用提示

1. **分支命名慣例**
   - 功能分支：`feature/功能名稱`
   - 修復分支：`bugfix/問題描述`
   - 發布分支：`release/版本號`

2. **提交信息格式**
   ```
   類型: 簡短描述

   詳細說明（如果需要）
   ```
   類型可以是：feat, fix, docs, style, refactor 等

3. **代碼審查清單**
   - 代碼是否遵循項目規範
   - 是否包含適當的測試
   - 文檔是否更新
   - 性能是否考慮

4. **常用操作快捷方式**
   - 創建新分支並切換：`git checkout -b 分支名`
   - 更新遠程分支：`git pull origin 分支名`
   - 查看分支狀態：`git status`

[其餘內容保持不變...]