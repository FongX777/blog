---
layout: post
title:  "How to use GCIN!"
date:   2017-05-20 16:00:27 +0800
categories: jekyll update
tags: [gcin][linux]
---


哈囉大家好，
今天來介紹的是一個我個人十分喜歡的中文輸入法：`Gcin`，
這套軟體是開源且免費的，
我在Linux Mint 上用起來十分的舒服，
在這邊分享一下如何使用！
Let's Go!

- 目錄：
1. [安裝][article-1]
2. [設定][article-2]
3. [個人化][article-3]

-------------------------------------------

1. 安裝
<a name="1"></a>
	首先，最重要的當然就是安裝囉~~
	因為這個輸入法在中文屆（主要針對繁體中文用戶）也算小有名氣，
	所以很多網誌都會分享如何安裝等等，
	但是！！！！！！
	很多都是古早以前寫的，所以如果你的Linux系統較前衛一點，
	要不就安裝失敗、要不就功能通通失靈，
	所以我鼓勵大家一律去找最新的安裝，
	最直接的就是上 [官方討論區][gcin-install-latest] 照步驟下載~

	若懶得點進去，請看下方~
	(1)取得認証金鑰
	   (若想了解更多...[點我][apt-key-introduce]）

		{% highlight ruby %}
		$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 835AB0E3
		{% endhighlight %}
	
	(2)新增進軟體來源(Software source)中
		可以打指令
		{% highlight ruby %}
		$ software-properties-gtk 
		{% endhighlight %}
		或是
		打開`Software Source`，

		然後到`其他軟體`（`Additional repositories`)中，
		`新增`(`Add`)
		{% highlight ruby %}
		deb http://hyperrate.com/gcin-ubuntu1604 eliu release
		{% endhighlight %}

		最後`更新`(`Update Cache`)後退出。

	(3) 安裝gcin
		{% highlight ruby %}
		$ sudo apt-get install gcin
		{% endhighlight %}

	(4) 安裝完成><
	

2. 設定
<a name="2"/>
	但不是安裝完就沒事了，
	你只是有這個軟體，但並不是系統預設的，
	因此如果是~
	(a)Ubuntu，
	右上角的齒輪→ 系統設定值→ 語言支援→ 鍵盤輸入法系統→ gcin
	或是執行 /usr/bin/gnome-language-selector→ 鍵盤輸入法系統→ gcin 
	(b)Mint
	menu → 進去input mehtod → input mehtod 選 gcin

	登出後回來gcin就出現了！！！

3. 個人化
<a name="3"/>
	當然，只是單純安裝還不能稱為好用的輸入法，
	一定要有一些個人化才行！
	
	(下集待續)


[article-1]: #1
[article-2]: #2
[article-3]: #3
[gcin-install-latest]:http://hyperrate.com/thread.php?tid=28044
[apt-key-introduce]:https://www.ubuntu-tw.org/modules/newbb/viewtopic.php?viewmode=compact&type=&topic_id=16902&forum=2



