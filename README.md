# Hugo + GitHub Pages 最小可用範例

這個專案讓你用 **Hugo** 產生靜態網站，並透過 **GitHub Actions** 部署到 **GitHub Pages**。

## 快速開始

1. 安裝 Hugo（macOS 例如：`brew install hugo`）。
2. 將本專案推到你的帳號：`BeStronger1983` 的使用者站點 repo：

   ```bash
   git init
   git add .
   git commit -m "init: hugo + pages"
   git branch -M main
   git remote add origin git@github.com:BeStronger1983/BeStronger1983.github.io.git
   git push -u origin main
   ```

3. 進到 GitHub → 該 repo → **Settings → Pages**，Source 選 **GitHub Actions**。幾十秒後會看到綠燈，站點網址：

   `https://BeStronger1983.github.io/`

> 若你準備自訂網域，請到 **Settings → Pages** 綁定；同時把 `hugo.toml` 的 `baseURL` 改為你的網域（含 `https://` ）。

## 本機開發

```bash
hugo server -D
```

## 新增文章

```bash
hugo new posts/my-first-post.md
# 編輯檔案後，記得把 front matter 裡的 draft 設為 false
```

## 備註
- 網站輸出在 `public/`，已加到 `.gitignore`。
- 模板是最小化的 `_default` 版面，之後你可以換主題或客製 `layouts/`。
