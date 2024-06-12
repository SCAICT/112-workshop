<!-- @format -->
<!-- .slide:class="r-fit-text" -->
# Linux 操作軟體

Each Chen


<!-- .slide:data-transition="fade-in slide-out" -->
---

## [MobaXterm](https:#mobaxterm.mobatek.net/download.html)

| <ul><li>視覺化 SSH client</li><li>連線管理、主機監控</li><li>有顏色的 CMD</li></ul> | ![MobaXterm](/slides/img/LinuxApplication/mobaxterm.jpg) <!-- .element: height="200px" -->|
|:---:|:-:|


--

## 安裝它 
<img class="r-stretch" src="/slides/img/LinuxApplication/installMobaxterm.jpg" />


--


## 建立連線
<img class="r-stretch" src="/slides/img/LinuxApplication/linkStart.png" />




--

## 其他 SSH 酷炫功能
- 主機資源監控
- Macrus
- 圖形化 Sftp





---

## Vim
- Unix 系統內建文字編輯器(更好用的記事本)
- 只用鍵盤的文字編輯器
- 在鍵盤上打 combo
- 插件多，自由度高



--

## 這有什麼用？
- Unix 系統裡面的預設文字編輯器
- 程式操作介面是 vim (git)
- ~~讓你看起來更像駭客~~
- ~~毛哥說不要教 nano~~



--

## 用 vim 開啟檔案
```
vim <fileNmae>
```



--

##  vim 指令(insert mode)
```
a(insert) #移動到游標字前面
i #移動到游標字後面
```



--

## vim 指令(command mode)
```

```


--

##  vim 指令(normal mode)
```
:q #放我出去
:w #儲存檔案
P/p #在上/下方一行貼上(從 vim 的)
d 剪下一行
x 剪下一個字(當刪除用)
yy 複製一行
```



--

## 移動指令
```
gg #移動到第一行
<number>gg #移動到第 number 行
G #移動到行尾
/<target> #向下尋找目標
N/n #向上/下尋找
0 #移動到該行最左邊
```



--

### 你可能不會用到的東西
#### vi的指令

```
hjkl #左下上右移動
``` 


--

### 教不完了，念指令好無聊，這些目前夠用了
[這裡有教學](https://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/)

---
<!-- .slide: data-background-image="/slides/img/LinuxApplication/boss.jpg" data-background-opacity="0.4" data-auto-animate -->
# process manager
##### 大統領，你是系統的主宰

--

## htop
```bat
foo@bar:~$ htop
```
![alt text](/slides/img/LinuxApplication/htopFull.png)
<!-- .slide:class="r-stretch" -->

--

## CPU
![alt text](/slides/img/LinuxApplication/htopDevice.png)
- 紅色(優先度高)
- 綠色
- 藍色(優先度低)

## 排程
- First-Come, First-Served(FCFS)
- Shortest-Job-First(SJF)
- Priority Scheduling

--
## 記憶體

![alt text](/slides/img/LinuxApplication/htopDevice.png)
- 記憶體 使用率
    - 綠色：被占用的
    - 藍色：buffer
    - 橘色：cache pages
- swap
    - 當記憶體用的硬碟空間

--

## 下面的東西

![alt text](/slides/img/LinuxApplication/htopProcess.png)