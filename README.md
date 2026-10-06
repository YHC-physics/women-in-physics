# 物理系女生小聚網站

這是一個純 HTML 網站，放在 GitHub Pages 上，任何人都能免登入瀏覽。編輯不需要 Claude，也不需要會寫程式。

## 檔案說明

| 檔案 | 用途 |
| --- | --- |
| `index.html` | 網站本身（一般不用改） |
| `content.js` | **網站上所有文字與照片清單都在這裡**，平常只需要更新這個檔案 |
| `edit.html` | 填表用的編輯頁，幫你產生正確的 `content.js`，避免打錯逗號或引號 |
| `photos/` | 放活動照片的資料夾 |

## 第一次架設（只要做一次，建議用電腦）

1. 到 github.com 註冊帳號。
2. 右上角「+」→ **New repository**，取個名字（例如 `physics-women`），選 **Public**，按 Create repository。
3. 在新頁面點 **uploading an existing file**（或 Add file → Upload files），把這個資料夾裡的所有檔案和 `photos` 資料夾拖進去，按 **Commit changes**。
4. 進入 **Settings → Pages**。在 Build and deployment 的 Source 選 **Deploy from a branch**，Branch 選 `main`，資料夾選 `/(root)`，按 **Save**。
5. 等一、兩分鐘，Pages 頁面上方會出現網站網址，通常是 `https://你的帳號.github.io/repo名稱/`。這就是要給新生的連結。

## 平常怎麼更新

### 更新文字、新增聚會或活動
1. 打開 `網站網址/edit.html`（例如 `https://你的帳號.github.io/physics-women/edit.html`）。
2. 修改內容，最後按 **產生 content.js**，再按 **複製全部**。
3. 到 GitHub 的 repo，點開 `content.js`，按右上角**鉛筆圖示**，全選、貼上，按 **Commit changes**。
4. 一、兩分鐘後，網站就會更新。

編輯頁會在瀏覽器裡暫存草稿，寫到一半關掉，下次打開可以選「載入草稿」。

### 新增照片
1. 在 `edit.html` 的「縮圖小工具」選照片，會自動縮小，逐張下載。
2. 到 GitHub 的 `photos` 資料夾，按 **Add file → Upload files**，上傳剛下載的照片，Commit。
3. 回到編輯頁，把小工具產生的檔案路徑貼到那個活動的「照片」欄，再照上面的步驟更新 `content.js`。

## 交接給下一任總召

- **簡單做法**：repo 的 **Settings → Collaborators → Add people**，輸入下一任的 GitHub 帳號，給她編輯權限。
- **長期建議**：建立一個 GitHub 組織（Organization，免費），把 repo 放在組織底下，歷任總召都加進組織。換人時只要新增、移除成員，網址和網站都不用動。
- 請用邀請的方式給權限，不要共用同一組帳號密碼。

## 注意事項

- 網站是公開的，任何人拿到連結都能看。
- 照片放上網前，請先徵得拍到的同學和老師同意。
- 不要放電話、學號等個人資料。
- 如果手動編輯 `content.js`，要小心引號和逗號；用 `edit.html` 產生比較不會出錯。
