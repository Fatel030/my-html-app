# 蔡宗諭 的個人網站與數位作品集 (my-html-app)

🌐 **線上網站**：[https://fatel030.github.io/my-html-app/](https://fatel030.github.io/my-html-app/)

歡迎來到我的個人數位展示空間！這裡是我記錄創作、分享程式碼與發表詩作的基地。

---

## 📂 專案檔案架構

```text
my-html-app/
├── index.html               # 個人主頁 / 數位名片與作品導覽
├── poetry.html              # 《蔡宗諭 詩集》線上數位紙張閱讀器 (新增)
├── poems.json               # 詩集資料庫 (由 build_poetry_database.py 自動生成)
├── build_poetry_database.py # 詩集資料庫提取與解析腳本
├── interactive_guide.html   # 社交與職場互動技能指南 (Dashboard 風格)
├── blog.html                # 部落格文章列表頁面
├── blog-post-1.html         # 部落格範例文章頁面
├── README.md                # 專案說明文件
└── assets/                  # 靜態資源資料夾
    ├── profile_photo.jpg    # 大頭照
    ├── resume.pdf           # 簡短履歷
    └── cv.pdf               # 詳細履歷
```

---

## 📖 詩集更新與發布工作流程 (Workflow)

當您在電腦本地（`F:\forwork\datafile\`）新增或修改詩作 `.docx` 檔案時，更新至線上網站的步驟如下：

1. **重新生成詩集資料庫**：
   在 PowerShell 或終端機中執行：
   ```bash
   python build_poetry_database.py
   ```
   *腳本會自動讀取資料夾並更新 `poems.json`。*

2. **推送到 GitHub Pages 發布**：
   ```bash
   git add .
   git commit -m "feat: 更新詩集作品與資料庫"
   git push origin main
   ```

3. **線上瀏覽**：
   推送完成後 1~2 分鐘，點擊 [https://fatel030.github.io/my-html-app/poetry.html](https://fatel030.github.io/my-html-app/poetry.html) 即可看到最新更新的詩集！
