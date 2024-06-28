# linux基礎教學
## 中電會113屆幹訓

---

# linux介紹
## What is linux?

----

## What is linux?
- 開源操作系統
- 使用UNIX開發(Mac OS也是!)
- 許多開源軟體、駭客工具都支援linux系統
- 允許多個使用者同時登入
- CLI介面

---

# linux基本指令
## 終於要開始了

---

## 基本指令- whoami、pwd
### 我是誰?我在哪?
- whoami-顯示使用者(沒啥用)
- pwd-顯示目前所在的目錄
![image](https://hackmd.io/_uploads/HkBbKP3HC.png)

---

## 基本指令- ls
- 查看當前目錄下的檔案
![image](https://hackmd.io/_uploads/HyrOFw2rC.png)

----

## 基本指令- ls
- 參數 -a
- 詳細顯示所有檔案，包括隱藏檔、檔案權限等等
- 參數 -l
- 垂直顯示列表
- 常見用法 ls-al

----

![image](https://hackmd.io/_uploads/rkQ8sPhHR.png)

---

## 基本指令- cd

- 切換資料夾路徑
- cd [資料夾路徑]
- 絕對路徑
![image](https://hackmd.io/_uploads/ByWprd2H0.png)

----

## 基本指令- cd
![image](https://hackmd.io/_uploads/HkYjwtnBR.png)

----

## 基本指令- cd
相對路徑
- ~ >家目錄
- .  >本層目錄
- ..>上層目錄
![image](https://hackmd.io/_uploads/rJSNKKhHA.png)

---

## 基本指令- cat
-輸出檔案內容
-cat [參數] [檔案路徑]
![image](https://hackmd.io/_uploads/Sy7Q2tnSR.png)

---

##  基本指令- mkdir
- 建立資料夾
- mkdir [資料夾路徑]
![image](https://hackmd.io/_uploads/HJPqaF3rA.png)

---

## 基本指令- vim、nano
先說，我是nano派的
![image](https://hackmd.io/_uploads/SkYoPc3rC.png)
![image](https://hackmd.io/_uploads/S1wAOcnH0.png)


----

##  NANO
- 簡單易用
- 預設安裝
- 適合新手(我就菜)

----

## NANO
- 打開就可以編輯
- ^X 是指 crtl+x
- 也可以建立程式檔
![image](https://hackmd.io/_uploads/BJ-HQ53SC.png)


----

## VIM
- 功能強大
- 整個鍵盤都是快捷鍵
- 較難上手

----

## VIM
- i : 編輯模式
- esc : 退出編輯模式
- :w 保存
- :q 退出
- :q! 強制退出
- :wq 保存加退出

----

![image](https://hackmd.io/_uploads/BJiHw5nr0.png)

---

## 基本指令- wget
- 下載網路檔案
- wget [參數] [網址]
- 參數 -O 下載檔案檔名
![image](https://hackmd.io/_uploads/ByPwochrC.png)

---

## 基本指令- ssh
- 連線至遠端的linux伺服器
- -p 連接端口
![image](https://hackmd.io/_uploads/BkPvhc2HA.png)

---

## 基本指令- sudo
- 以最高權限執行
- sudo [指令]
![image](https://hackmd.io/_uploads/rkvjpchBR.png)

---

## 基本指令- chmod
![螢幕擷取畫面 2024-06-17 012205](https://hackmd.io/_uploads/rkY_JinHR.png)

----

## 基本指令- chmod
![螢幕擷取畫面 2024-06-17 012119](https://hackmd.io/_uploads/r1hYyo3H0.png)

----

## 基本指令- chmod
![image](https://hackmd.io/_uploads/S1h1ljhBR.png)


----

## 基本指令- chmod
![image](https://hackmd.io/_uploads/H14GxjnBC.png)

---

## 基本指令- man
- 查詢其他指令的方法
- man [指令]

---

# 謝謝大家