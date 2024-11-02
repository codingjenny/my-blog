+++
date = '2024-10-29T13:00:49+08:00'
draft = false
title = 'Hugo - 快速了解 Hugo 使用方法'
+++
## Hugo - 快速了解 Hugo 使用方法

Hugo 是一個靜態網站生成器，可以用來快速建立個人網站。

在 Hugo 的官網上可以找到 [Quick start](https://gohugo.io/getting-started/quick-start/) 的教學。本篇的存在意義是記錄我學習 Hugo 的過程，以及給不想直接看英文檔案的人參考 😎。

透過本篇的教學，你將會學到：

1. 如何安裝 Hugo
2. 如何建立一個新的網站
3. 如何新增文章
4. 如何新增頁面
5. 如何使用 Hugo 的 theme

把這幾項做完，就可以差不多了解 Hugo 的使用方法。

---------------
### 安裝 Hugo

這裡只會講 Mac OS 安裝 Hugo 的方法，其他作業系統的安裝方法可以參考 [Hugo Installation](https://gohugo.io/getting-started/installing/)。

我是用 Homebrew 安裝 Hugo，如果沒有 Homebrew 可以參考 [Homebrew Installation](https://brew.sh/)，內建繁體中文翻譯。

Homebrew 安裝完後，就可以用以下指令安裝 Hugo：

```bash
brew install hugo
```

想確認 Hugo 是否安裝成功，可以執行以下指令：

```bash
hugo version
```

如果出現版本資訊，就代表安裝成功。類似：

```bash
hugo v0.136.5+extended darwin/arm64 BuildDate=2024-10-24T12:26:27Z VendorInfo=brew
```

---------------
### 建立一個新的網站

我會先切換終端機到想放置資料夾的位置，但如果你就是想放在目前的位置，就直接執行以下指令：

```bash
# chanlee-blog 是我自己取的，可以改成你想要的資料夾名稱
hugo new site chanlee-blog
```
這個指令會直接在根目錄建立一個名為 chanlee-blog 的資料夾，裡面會有建立好的檔案結構。

切換到剛剛建立的資料夾：

```bash
cd chanlee-blog
```

```bash
git init
```

```bash
git clone https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
```

```bash
echo "theme = 'ananke'" >> hugo.toml
```

```bash
hugo server
```
