<!-- .slide:class="r-fit-text" -->
# Linux 操作軟體

Each Chen

---

<!-- .slide:data-transition="fade-in slide-out" -->
<!-- .slide:class="r-fit-text" -->
<section>

## [MobaXterm](https:#mobaxterm.mobatek.net/download.html)

| <ul><li>視覺化 SSH client</li><li>連線管理、主機監控</li><li>有顏色的 CMD</li></ul> | ![MobaXterm](/slides/img/LinuxApplication/mobaxterm.jpg) <!-- .element: height="200px" -->|
|:---:|:-:|

</section>
<!-- .slide:class="r-fit-text" -->
<section>

## 安裝它 
<img class="r-stretch" src="/slides/img/LinuxApplication/installMobaxterm.jpg" />

</section>
<!-- .slide:class="r-fit-text" -->
<section>

## 建立連線
<img class="r-stretch" src="/slides/img/LinuxApplication/linkStart.png" />


</section>

<section>

## 其他 SSH 酷炫功能
- 主機資源監控
- Macrus
- 圖形化 Sftp

</section>


---

<section>

## Vim
- Unix 系統內建文字編輯器(更好用的記事本)
- 只用鍵盤的文字編輯器
- 在鍵盤上打 combo
- 插件多，自由度高

</section>

<section>

## 這有什麼用？
- Unix 系統裡面的預設文字編輯器
- 程式操作介面是 vim (git)
- ~~讓你看起來更像駭客~~
- ~~毛哥說不要教 nano~~

</section>

<section>

## 用 vim 開啟檔案
```
vim <fileNmae>
```

</section>

<section>

##  vim 指令(insert mode)
```
a(insert) #移動到游標字前面
i #移動到游標字後面
```

</section>

<section>

## vim 指令(command mode)
```

```
</section>

<section>

##  vim 指令(normal mode)
```
:q #放我出去
:w #儲存檔案
P/p #在上/下方一行貼上(從 vim 的)
d 剪下一行
x 剪下一個字(當刪除用)
yy 複製一行
```

</section>

<section>

## 移動指令
```
gg #移動到第一行
<number>gg #移動到第 number 行
G #移動到行尾
/<target> #向下尋找目標
N/n #向上/下尋找
0 #移動到該行最左邊
```

</section>

<section>

# 你可能不會用到的東西
### vi的指令

```
hjkl #左下上右移動
``` 

</section>
<!-- .slide:class="r-fit-text" -->
<section>

### 教不完了，念指令好無聊，這些目前夠用了
[這裡有教學](https://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/)
</section>