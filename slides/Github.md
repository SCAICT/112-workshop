# Git & GitHub
中部電資聯合會議幹訓

![scaict](../slides/img/GitHub/icon.png)

---

### 不知道要不要放的自我介紹

<img style="float: left; height:300px; margin-left: 100px;" src="https://hackmd.io/_uploads/S14lQa9rA.jpg">

<ul style="margin-top: 30px">
    <li>邱德原(De-Yuan, Chiu)</li>
    <li>台中一中電研社教學</li>
    <li>SCAICT 資訊組</li>
    <li>也可以叫我ChiuChiuCircle</li>
    <li style="font-size:35px;">https://chiudeyuan.github.io/</li>    
</ul>

---

### 先備知識
* 基礎cmd使用

---

## 認識Git
![](../slides/img/GitHub/git.png)

--

### Git是一種版本控制器（VCS）
Git由Linus Torvalds開發

![](../slides/img/GitHub/VSC.png)<!-- .element: height="400px" -->

--

### 版本控制的好處

* 追踪變更記錄
* 恢復檔案
* 資料備份
* 方便比較差異
* 工作流管理

--

### 分支 Branch

![](../slides/img/GitHub/branch.png)

基本上Git的概念就是在開發與合併branch

--

### 冷知識
Git在英國俚語是指"不愉快的人"
因為Linus不爽Bitkeeper(也是VCS)收回他的免費使用權

![](../slides/img/GitHub/meme1.jpg)<!-- .element: height="400px" -->

---

## GitHub
![](../slides/img/GitHub/github.png)

--

### GitHub是用來存放Git的空間
![](../slides/img/GitHub/github1.png)<!-- .element: height="400px" -->

--

### GitHub的好處

* 方便管理專案
* 支持多人協作
* 促進開源風氣

---

## GitHub基本概念

--

![](../slides/img/GitHub/basic1.png)

--

### 1. Repository
存放程式碼的地方
![](../slides/img/GitHub/github2.png)

--

長這樣

![](../slides/img/GitHub/github1.png)<!-- .element: height="400px" -->

--

按New建立新Repo

![](../slides/img/GitHub/basic2.png)<!-- .element: height="400px" -->

--

填Repo的一些資料

![](../slides/img/GitHub/basic3.png)<!-- .element: height="500px" -->

--

### 2. Clone
將Repository複製到本機以進行修改

![](../slides/img/GitHub/github3.png)

--

GitHub上的Repositorty

![](../slides/img/GitHub/basic4.png)

--

按下"Code"後會有一串網址

我們用這個網址進行clone

![](../slides/img/GitHub/basic5.png)

--

在cmd使用指令clone

注意"Repo網址"是剛剛的那個網址

不是GitHub頁面的網址
```
git clone [Repo網址]
```

--

clone下來後本機就會多出一個資料夾

![](../slides/img/GitHub/basic6.png)<!-- .element: height="400px" -->

--

### 3. Pull
如果本機原本就已經有Repo

能用Pull獲得GitHub上的最新版本

![](../slides/img/GitHub/github3.png)

--

在本機的資料夾中的cmd使用指令
```
git pull
```

--

### 4. Fork 
將別人的Repository複製一份給自己

這樣就能在不影響Origin的狀況下自由開發

![](../slides/img/GitHub/github4.png)

--

在別人的Repo裡會有這個按鈕

![](../slides/img/GitHub/basic7.png)

--

按下去就能建立Forked Repo

![](../slides/img/GitHub/basic8.png)

--

### 5. Push
當修改完程式碼

就能上傳到GitHub上的Repo
![](../slides/img/GitHub/github5.png)

--

在本機的資料夾中的cmd使用指令
```
git push
```

--

### 6. Pull Request
如果你是協作他人專案

可以通過PR貢獻自己的code

![](../slides/img/GitHub/github6.png)

--

### 6. Pull Request
如果對方覺得你給的code還行

就會把code合併進他們的專案中

並把你列為協作者

---

## Git的使用 | 前置作業

--

### 下載Git

https://www.git-scm.com/downloads

![](../slides/img/GitHub/download1.png)<!-- .element: height="500px" -->

--

可以用指令確認是否安裝成功
```
git --version
```

--

### 與GitHub連線

--

### 一、GitHub Desktop
登入GitHub Desktop就能直接控制Repo

https://desktop.github.com/

![](../slides/img/GitHub/download2.png)<!-- .element: height="500px" -->

--

### 二、使用SSH Key

也能通過SSH Key授權控制Repo

(如果有GitHub Desktop可以不用)

--

#### 1. 在PowerShell輸入生成金鑰指令
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

--

應該會有一些可以設定密碼的選項

還有確認密鑰檔案儲存位置

接著密鑰就生成好了

![](../slides/img/GitHub/ssh1.png)<!-- .element: height="400px" -->

--

#### 2. 上傳公鑰

因為SSH有公私鑰

我們是要將「公鑰」上傳至GitHub

在儲存密鑰的資料夾中輸入指令
```
cat .\id_ed25519.pub
```

--

我們將整段文字複製起來

從ssh-ed25519一直到email都要

![](../slides/img/GitHub/ssh2.png)

--

到GitHub的setting裡找到SSH設定

![](../slides/img/GitHub/ssh3.png)<!-- .element: height="500px" -->

--

按下new ssh key後把公鑰貼上就完成了

![](../slides/img/GitHub/ssh4.png)

--

之後clone或push都是使用SSH

![](../slides/img/GitHub/ssh5.png)<!-- .element: height="500px" -->

---

## Git的使用 | 各種操作

--


+ 初始化資料夾
    * init & remote
    * clone
+ commit
+ branch
+ push
+ pull

--

### 1. init & remote

把一個資料夾設置為git追蹤的對象
```
git init
```

--

但在init後要選擇控制哪個Repo
所以用指令remote

```
git remote add origin [Repo網址]
```

這邊add指的是「新增控制的目標」

origin是remote端的「別稱」

--

![](../slides/img/GitHub/meme2.png)<!-- .element: height="700px" -->

--

我們通常將remote端（如GitHub）稱為Origin

![](../slides/img/GitHub/usage1.png)

--

### 2. clone
使用指令複製Repo至本地
```
git clone [Repo URL]
```
![](../slides/img/GitHub/usage2.png)

--

### commit
當我們完成修改後

就要把這個版本記錄起來

![](../slides/img/GitHub/usage3.png)<!-- .element: height="500px" -->

--

### commit
使用指令
```
git commit -m "something"
```
參數「-m」是指有附加此commit的訊息

後面的「"something"」便是附加訊息

可以讓人一眼看出此版本有什麼改動

--

就能成功紀錄新版本

![](../slides/img/GitHub/usage3.png)<!-- .element: height="500px" -->

--

就能成功紀錄新版本

![](../slides/img/GitHub/usage4.png)<!-- .element: height="500px" -->

--

### branch & checkout
先前有說過Git可以在不同分支上進行開發

![](../slides/img/GitHub/branch.png)

--

使用指令查看目前分支
```
git branch
```

--

星號「*」是用於標示目前在哪一個branch上

![](../slides/img/GitHub/usage5.png)<!-- .element: height="500px" -->

--

開啟新分支指令
```
git branch [branch_name]
```

--

開啟新分支

![](../slides/img/GitHub/usage5.png)<!-- .element: height="500px" -->

--

開啟新分支

![](../slides/img/GitHub/usage6.png)<!-- .element: height="500px" -->

--

再利用checkout切換目前所在branch
```
git checkout [branch_name]
```

--

![](../slides/img/GitHub/usage6.png)<!-- .element: height="500px" -->

--

![](../slides/img/GitHub/usage7.png)<!-- .element: height="500px" -->

--

### merge
~~Git中的大魔王~~

合併branch

--

當我們在branch上做了一些開發

最後會需要將分支合併起來

![](../slides/img/GitHub/usage8.png)<!-- .element: height="500px" -->

--

使用merge指令
```
git merge [被合併branch_name]
```

--

但要注意在合併前要先在正確的branch

![](../slides/img/GitHub/usage8.png)<!-- .element: height="500px" -->

--

例如要將B merge到main

![](../slides/img/GitHub/usage8.png)<!-- .element: height="500px" -->

--

就要先checkout到main上

![](../slides/img/GitHub/usage9.png)<!-- .element: height="500px" -->

--

然後再merge

![](../slides/img/GitHub/usage10.png)<!-- .element: height="500px" -->

--

<iframe width="973" height="695" src="https://www.youtube.com/embed/dygYh2qsx64" title="when git merge 😂😂😂 #git #programming memes" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

--

### push
完成工作後

要將code上傳至GitHub

--

使用指令
```
git push
```
或
```
git push origin master
```

--

![](../slides/img/GitHub/usage5.png)<!-- .element: height="500px" -->

--

![](../slides/img/GitHub/usage11.png)<!-- .element: height="500px" -->

--

![](../slides/img/GitHub/meme3.png)<!-- .element: height="500px" -->

--

### pull
更新本機上的檔案

--

例如remote端多了一個新的commit

![](../slides/img/GitHub/usage12.png)<!-- .element: height="500px" -->

--


使用指令
```
git pull
```

--

檔案就能更新到remote端的版本

![](../slides/img/GitHub/usage13.png)<!-- .element: height="500px" -->

---

最後推薦一個學Git的網站
https://learngitbranching.js.org/?locale=zh_TW

---

## 謝謝聆聽

![](../slides/img/GitHub/meme4.jpg)<!-- .element: height="500px" -->

