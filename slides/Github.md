# Git & GitHub
中部電資聯合會議幹訓
![.](../img/GitHub/icon.png)

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
![a0129](https://hackmd.io/_uploads/ryg6NFVcT.jpg =60%x)

----

### Git是一種版本控制器（VCS）
Git由Linus Torvalds開發
![local](https://hackmd.io/_uploads/Bk4zfAcHA.png =60%x)

----

### 版本控制的好處

* 追踪變更記錄
* 恢復檔案
* 資料備份
* 方便比較差異
* 工作流管理

----

### 分支 Branch

![螢幕擷取畫面 2024-06-15 164918](https://hackmd.io/_uploads/H1woB09SA.png)
基本上Git的概念就是在開發與合併branch

----

### 冷知識
Git在英國俚語是指"不愉快的人"
因為Linus不爽Bitkeeper(也是VCS)收回他的
免費使用權
![xsdtv](https://hackmd.io/_uploads/SkoUWNyIA.jpg)

---

## GitHub
![github-logo](https://hackmd.io/_uploads/BJBmLkjSC.png)

----

### GitHub是用來存放Git的空間
![螢幕擷取畫面 2024-06-15 181127](https://hackmd.io/_uploads/S1fJt1or0.png =50%x)

----

### GitHub的好處

* 方便管理專案
* 支持多人協作
* 促進開源風氣

---

## GitHub基本概念

----

![git-github-workflow-1000w](https://hackmd.io/_uploads/r1JPwEiHC.png =80%x)

----

### 1. Repository
存放程式碼的地方
![sfdghfghjfghj](https://hackmd.io/_uploads/B1Ik_NorA.png =80%x)

----

長這樣
![螢幕擷取畫面 2024-06-15 181127](https://hackmd.io/_uploads/S1fJt1or0.png =50%x)

----

按New建立新Repo
![螢幕擷取畫面 2024-06-16 002512](https://hackmd.io/_uploads/BkzCxBjBA.png)

----

填Repo的一些資料
![螢幕擷取畫面 2024-06-16 002533](https://hackmd.io/_uploads/Bk1xZSiSR.png =60%x)

----

### 2. Clone
將Repository複製到本機以進行修改
![sfdghfghjfghj](https://hackmd.io/_uploads/HkFId4jHA.png =80%x)

----

GitHub上的Repositorty

![螢幕擷取畫面 2024-06-16 000319](https://hackmd.io/_uploads/r1yYjNsr0.png)

----

按下"Code"後會有一串網址
我們用這個網址進行clone
![螢幕擷取畫面 2024-06-16 002233](https://hackmd.io/_uploads/rJCAbBsrA.png)

----

在cmd使用指令clone
注意"Repo網址"是剛剛的那個網址
不是GitHub頁面的網址
```
git clone [Repo網址]
```

----

clone下來後本機就會多出一個資料夾

![螢幕擷取畫面 2024-06-16 000646](https://hackmd.io/_uploads/HJWwnVjBC.png =20%x)

----

### 3. Pull
如果本機原本就已經有Repo
能用Pull獲得GitHub上的最新版本
![sfdghfghjfghj](https://hackmd.io/_uploads/HkFId4jHA.png =80%x)

----

在本機的資料夾中的cmd使用指令
```
git pull
```

----

### 4. Fork 
將別人的Repository複製一份給自己
這樣就能在不影響Origin的狀況下自由開發
![sfdghfghjfghj](https://hackmd.io/_uploads/ryyJTNirR.png =80%x)

----

在別人的Repo裡會有這個按鈕

![螢幕擷取畫面 2024-06-16 001546](https://hackmd.io/_uploads/HJFDCNoHC.png)

----

按下去就能建立Forked Repo

![螢幕擷取畫面 2024-06-15 231644](https://hackmd.io/_uploads/r15PSVsr0.png)

----

### 5. Push
當修改完程式碼
就能上傳到GitHub上的Repo
![git-github-workflow-1000w](https://hackmd.io/_uploads/B14j4BsH0.png =80%x)

----

在本機的資料夾中的cmd使用指令
```
git push
```

----

### 6. Pull Request
如果你是協作他人專案
可以通過PR貢獻自己的code
![git-github-workflow-1000w](https://hackmd.io/_uploads/Syd-DrjrA.png =80%x)

----

### 6. Pull Request
如果對方覺得你給的code還行
就會把code合併進他們的專案中
並把你列為協作者
![git-github-workflow-1000w](https://hackmd.io/_uploads/Syd-DrjrA.png =80%x)

---

## Git的使用 | 前置作業

----

### 下載Git

https://www.git-scm.com/downloads
![螢幕擷取畫面 2024-06-17 200850](https://hackmd.io/_uploads/HyTdDjar0.png =60%x)

----

可以用指令確認是否安裝成功
```
git --version
```

----

### 與GitHub連線

----

### 一、GitHub Desktop
登入GitHub Desktop就能直接控制Repo

https://desktop.github.com/
![螢幕擷取畫面 2024-06-17 202814](https://hackmd.io/_uploads/HyClniTrC.png =60%x)

----

### 二、使用SSH Key

也能通過SSH Key授權控制Repo
(如果有GitHub Desktop可以不用)

----

#### 1. 在PowerShell輸入生成金鑰指令
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

----

應該會有一些可以設定密碼的選項
還有確認密鑰檔案儲存位置
接著密鑰就生成好了

![螢幕擷取畫面 2024-06-17 223249](https://hackmd.io/_uploads/r14ucTpSR.png)

----

#### 2. 上傳公鑰

因為SSH有公私鑰
我們是要將「公鑰」上傳至GitHub
在儲存密鑰的資料夾中輸入指令
```
cat .\id_ed25519.pub
```

----

我們將整段文字複製起來
從ssh-ed25519一直到email都要
![螢幕擷取畫面 2024-06-17 224338](https://hackmd.io/_uploads/rkF7266H0.png)

----

到GitHub的setting裡找到SSH設定
![螢幕擷取畫面 2024-06-17 224707](https://hackmd.io/_uploads/SJin3aaHA.png)

----

按下new ssh key後把公鑰貼上就完成了
![螢幕擷取畫面 2024-06-17 224844](https://hackmd.io/_uploads/HJqN6TpB0.png)

----

之後clone或push都是使用SSH

![螢幕擷取畫面 2024-06-17 225223](https://hackmd.io/_uploads/r1uyRpTr0.png)

---

## Git的使用 | 各種操作

----


+ 初始化資料夾
    * init & remote
    * clone
+ commit
+ branch
+ push
+ pull

----

### 1. init & remote

把一個資料夾設置為git追蹤的對象
```
git init
```

----

但在init後要選擇控制哪個Repo
所以用指令remote

```
git remote add origin [Repo網址]
```
>這邊add指的是「新增控制的目標」
>origin是Repo的「別稱」

----

![5iphhycu0io11](https://hackmd.io/_uploads/SyLR-4y8C.png =50%x)

----

我們通常將remote端（如GitHub）稱為Origin
![scaict.drawio (3)](https://hackmd.io/_uploads/SyJWX1RBR.png =60%x)

----

### 2. clone
使用指令複製Repo至本地
```
git clone [Repo URL]
```
![scaict.drawio (4)](https://hackmd.io/_uploads/BynOXJ0SC.png =60%x)

----

### commit
當我們完成修改後
就要把這個版本記錄起來
![scaict.drawio (5)](https://hackmd.io/_uploads/BkIA2RCSA.png =60%x)

----

### commit
使用指令
```
git commit -m "something"
```
>參數「-m」是指有附加此commit的訊息
>後面的「"something"」便是附加訊息
>可以讓人一眼看出此版本有什麼改動

----

就能成功紀錄新版本
![scaict.drawio (5)](https://hackmd.io/_uploads/BkIA2RCSA.png =60%x)

----

就能成功紀錄新版本
![scaict.drawio (6)](https://hackmd.io/_uploads/rkawbMy80.png =60%x)

----

### branch & checkout
先前有說過Git可以在不同分支上進行開發
![螢幕擷取畫面 2024-06-15 164918](https://hackmd.io/_uploads/H1woB09SA.png)

----

使用指令查看目前分支
```
git branch
```

----

星號「*」是用於標示目前在哪一個branch上

----

開啟新分支指令
```
git branch [branch_name]
```

----

開啟新分支
![scaict.drawio (8)](https://hackmd.io/_uploads/HygNfm1IA.png =60%x)

----

開啟新分支
![scaict.drawio (9)](https://hackmd.io/_uploads/BkUrzQyIC.png =60%x)

----

再利用checkout切換目前所在branch
```
git checkout [branch_name]
```

----

![scaict.drawio (9)](https://hackmd.io/_uploads/BkUrzQyIC.png =60%x)

----

![scaict.drawio (10)](https://hackmd.io/_uploads/ByhCMXkL0.png =60%x)

----

### merge
~~Git中的大魔王~~
合併branch

----

當我們在branch上做了一些開發
最後會需要將分支合併起來
![scaict.drawio (11)](https://hackmd.io/_uploads/BJKp7Qk8A.png =60%x)

----

使用merge指令
```
git merge [被合併branch_name]
```

----

但要注意在合併前要先在正確的commit點
![scaict.drawio (11)](https://hackmd.io/_uploads/BJKp7Qk8A.png =60%x)

----

例如要將B2 merge到V2
![scaict.drawio (11)](https://hackmd.io/_uploads/BJKp7Qk8A.png =60%x)

----

就要先checkout到V2上
![scaict.drawio (12)](https://hackmd.io/_uploads/Bk8WwmJ8C.png =60%x)

----

然後再merge
![scaict.drawio (13)](https://hackmd.io/_uploads/ryqED7yUA.png =50%x)

----

<iframe width="973" height="695" src="https://www.youtube.com/embed/dygYh2qsx64" title="when git merge 😂😂😂 #git #programming memes" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

----

### push
完成工作後
要將code上傳至GitHub

----

使用指令
```
git push
```
或
```
git push origin master
```

----

![scaict.drawio (6)](https://hackmd.io/_uploads/SJEenmkL0.png =60%x)

----

![scaict.drawio (15)](https://hackmd.io/_uploads/SkJV3Q1U0.png =60%x)

----

![115881109_748798125903588_5372953434776795175_n](https://hackmd.io/_uploads/SydIMVkLA.png =60%x)

----

### pull
更新本機上的檔案

----

例如remote端多了一個新的commit
![scaict.drawio (16)](https://hackmd.io/_uploads/r1gRaQ1I0.png =50%x)

----


使用指令
```
git pull
```

----

檔案就能更新到remote端的版本
![scaict.drawio (17)](https://hackmd.io/_uploads/BJYPA7yUR.png =50%x)

---

最後推薦一個學Git的網站
https://learngitbranching.js.org/?locale=zh_TW

---

## 謝謝聆聽

![Fr7GWJ0WcBIvCIc](https://hackmd.io/_uploads/S1kwrEyUR.jpg =50%x)


