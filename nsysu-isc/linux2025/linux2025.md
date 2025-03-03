---
marp: true
theme: uncover
class: invert
paginate: true
---
<!-- style: ".left-txt {margin-right: -150px;font-size: 32px;}" -->

# Beginner's Guide to Linux for Information Security 
By Khin (Zin) Wang

---

### 今天有人沒有攜帶隨身碟嗎？


---

![](./assets/badbad.png)

---

### 開始之前，先問大家有沒有看過這個畫面

![fit](./assets/bs.jpg)


---

### Outline
1. What Is Linux?
2. Why Linux?
3. How To Start?
4. Let's Play With Kali Linux!

---

# What Is Linux? 😲

---
### What is Linux?

* Linux 是一種有別於 Windows 與 MacOS 的作業系統

---

### 被廣泛應用於

* 超級電腦：市場佔比 100% (前500 強超級電腦)
* 伺服器：市場佔比 62.7%
* 手機：市場佔比 73% (Android) 🤔
* 嵌入式設備：市場佔比 38.42%
* 其他種種設備


---
## 例如
--- 
### [路由器](https://www.asus.com/tw/networking-iot-servers/wifi-routers/asus-wifi-routers/rt-ac1500g-plus/)
![bg width:450px left](./assets/router.png)

--- 
### [3D 列印機](https://www.raspberrypi.com/success-stories/formlabs-3d-printers/)
![bg width:600px right](./assets/3dprinter.png)

---
### [工業控制器](https://www.raspberrypi.com/success-stories/industrial-shields-plcs/)
![bg width:500px left](./assets/plc.jpg)

---
### [電子看板](https://mastodon.social/@itsfoss/113843582408089244)
![bg right](./assets/train.jpeg)

---

### [遊戲機](https://www.steamdeck.com/zh-tw/tech)
![bg fit left](./assets/steamdeck.jpg)

---
### [樹莓派](https://www.raspberrypi.com/)
![bg right](./assets/rbpie.jpg)

---
### 還有爸爸!!
![bg width:800px left](./assets/jenson.jpg)

---
### ...手上的 <br> [Jetson Nano](https://www.youtube.com/watch?v=dHvb225Pw1s)
![bg width:800px left](./assets/jetson.png)

---

## 除了...

---

## PC 與筆電：市場佔比 4.1%

---

### 紀錄片：<br>[作業系統革命](https://www.youtube.com/watch?v=vWwvh3036Fw)
![bg width:450px left](./assets/revoltos.jpg)

---
## Linux 的誕生
---
## Linux 之父： <br> Linus Torvalds

---

### Linus Torvalds

![bg width:350px left](./assets/linus.webp)


<div class="left-txt">


+ 出生於芬蘭赫爾辛基市
+ 赫爾辛基大學計算機科學系畢業
+ 只用十天時間開發出 Git 的天才
+ Linux 核心始作俑者

</div>

---
### 回顧歷史：最初的開端
[Hello everybody out there using minix](https://groups.google.com/g/comp.os.minix/c/dlNtH7RRrGA/m/SwRavCzVE7gJ)

---

![bg 90%](./assets/linuxinit0.png)

---

![bg 90%](./assets/linuxinit1.png)

---

![bg 90%](./assets/linuxinit2.png)

---

![bg 90%](./assets/linuxinit3.png)

---

![](./assets/tough.png)

---

## 同一時期大西洋的另一端：<br>GNU 計劃

---
### 自由軟體社群的奮鬥： [GNU 計劃](https://zh.wikipedia.org/zh-tw/GNU%E8%A8%88%E5%8A%83)

+ GNU for GNU's Not Unix
+ 源自於自由軟體基金會
+ 主張公開共享原始碼，任何人都能自由修改、發佈
+ 希望開發出一款自由的作業系統，替代專有 Unix 系統

---

## 然而自由軟體社群遭遇一個巨大瓶頸 😱



---

## GNU 的作業系統核心 [Hurd](https://zh.wikipedia.org/zh-tw/GNU_Hurd) 難產 🥶

---

![bg width:350px left](./assets/linuxthug.png)

此時隔著大西洋另一岸的某個 21 歲芬蘭大學生剛好寫了一個作業系統核心

---

![bg 45%](./assets/hurdmeme.jpg)

---

## [Just For Fun - Linux Torvalds](https://www.tenlong.com.tw/products/9780066620732)

![](./assets/jsutforfun.jpg)

---

### 所以技術上來說,<br>Linus 當初開發的 Linux 作業系統<br>**不等於**現今口語說的 Linux 系統


---

### Linus 開發的是作業系統核心

>  作業系統唯一的使命就是幫助其它程式執行，
   所以作業系統從未獨立運行，而僅是默默等待程式，
   來向它要求現有資源、某個存在硬碟上的檔案，
   或要求其它程式，將這個程式連接到外面去，
   然後作業系統再一步步地，試著讓人們寫程式容易一些。
   -- Linux Torvalds
---

## 那我們口語中說的 Linux 系統<br>又是什麼？

---
## Linux 發行版/Linux Distro 

---
## 應用程式 + Linux 作業系統核心

---
### + Linux 作業系統核心

![bg contain left](./assets/xfce.png)



---

## [Linux 發行版有那些？](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg) 🤷

---

## Debian 家族

![bg right 86%](./assets/debian.jpg)
![bg 100%](./assets/ubuntu.png)
![bg 100%](./assets/mint.png)
![bg 100%](./assets/kali.png)
![bg 100%](./assets/rbpielogo.png)
+ [Debian](https://www.debian.org/)
+ [Ubuntu](https://ubuntu.com/)
+ [Mint](https://linuxmint.com/)
+ [Kali Linux](https://www.kali.org/)
+ [Raspberry Pi OS](https://www.raspberrypi.com/software/)
+ ...

---

## Arch 家族

![bg right 70%](./assets/arch.png)
![bg 65%](./assets/manjaro.png)
![bg 100%](./assets/blackarch.png)


+ [Arch](https://archlinux.tw/)
+ [Manjaro](https://manjaro.org/)
+ [BlackArch](https://blackarch.org/)
+ ...

---

## RedHat 家族

![bg right 86%](./assets/fedora.png)
![bg 90%](./assets/centos.png)
![bg 95%](./assets/redhat.png)

+ [Fedora](https://fedoraproject.org/zh-Hant/)
+ [CentOS](https://www.centos.org/) (已停止開發)
+ [RHEL](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux) (企業付費版)
+ ...

---

## 其他

![bg right 86%](./assets/gentoo.png)
![bg 100%](./assets/opensuse.png)

+ [Gentoo](https://www.gentoo.org/)
+ [openSUSE](https://www.opensuse.org/)
+ ...

---

# Why Linux? 🤨

---

## 在這之前，我想自我反省一下： <br> [推廣 Linux 的態度](https://archlinux.tw/getting-started/)


---

![bg fit](./assets/whyarch.png)

---

## 好，回到主題 😇

---

### 為什麼使用 Linux? 🤔

1. 大多免費🤩
2. 開放原始碼🙌
3. 自訂程度超高🧑‍🔧
4. 硬體資源需求低💻

---

### 1. 大多免費 🤩

#### 沒錯！ 大部分[發行版](https://upload.wikimedia.org/wikipedia/commons/1/1b/Linux_Distribution_Timeline.svg)都免費，<br>而且選擇超級無敵多！太幸福了!

---

### 許多使用者(包含我XD)<br>都會染上換換病<br>每隔一段時間不換個發行版，<br>渾身不自在🥵

---

### 2. 開放原始碼 🙌

+ 推陳出新超快，遇到 Bug 修復也超快！
+ 原始碼一切都是公開透明，不怕有人[衝康](https://www.informationsecurity.com.tw/article/article_detail.aspx?aid=11018)！安全有保障！ 
+ 有超龐大的愛好者社群，遇到問題不用怕！新手也免驚！
+ 有超多愛好者奉獻熱情開發並與大家分享，你也可以！

---

### 3. 自訂程度超高 🧑‍🔧

+ 真正感受到，你的電腦是你的電腦！
+ 各種功能都可以按照喜好自訂，讓電腦變成你的形狀！😈
+ Linux 世界裡，沒有什麼是你不能做的！(包含自我毀滅)
+ 遇到問題可親自動手解決，想要什麼功能也能自己來寫！

---

### 假如你不喜歡原本的[桌面環境](https://xtom.com/blog/the-10-best-linux-desktop-environments/)?<br>換！都換！👍

---

![bg fit left:80%](./assets/cinnamon.webp)
### 這樣

---

![bg fit right:80%](./assets/xfce.webp)
### 這樣

---

![bg fit left:80%](./assets/budgie.jpg)
### 還是這樣

---

### 假如你不喜歡原本的[檔案管理器](https://www.tecmint.com/linux-file-managers/)?<br>換！都換！🤙

---


### 假如你不喜歡原本的[音效伺服器](https://runmodule.com/2021/12/11/linux-sound-servers/)?<br>換！都換！💪

---



### 4. 硬體資源需求低💻

+ 資源使用效率高，更能發揮電腦性能
+ 適合運行在硬體資源有限之嵌入式、邊緣設備🤖
+ 可以運行在久遠以前的舊電腦

---


### 例子：[大神](https://youtu.be/L8XOqrKBM5w?feature=shared)用一堆回收場蒐集來的舊設備<br>運行 Linux，竊聽氣象衛星訊號📡

---


# How To Start?


---

## 1. 先體驗看看

+ 虛擬機
+ Live USB 
![](./assets/liveusb.png)

+ 先從圖像介面開始
+ [Linux 初學者應該知道的事](https://forum.gamer.com.tw/Co.php?bsn=60030&sn=2427798)

---

如果覺得好像可以的話🤔

---

## 2. 慢慢熟悉操作

+ 慢慢從做中學
+ 文件、社群可問

---

如果覺得好像可以的話🤔

---

## 3. 安裝雙系統或直接使用

---

## 心理建設

---

+ 遇到問題

---


# Let's Play With Kali Linux!🥳


---

## 最後補充個小知識

---

### Linux 的吉祥物是一隻<br>企鵝，叫做 Tux

![bg width:80% left:40%](./assets/tux.svg)

---

### 據說由來是 Linus Torvalds 在澳洲旅遊時，被動物園的一隻企鵝咬了一口

![](./assets/penguin.png)

---

## Thank You!

![bg contain left](./assets/car.png)