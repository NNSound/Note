# Note
稍微紀錄一下學習心得、筆記  

2018/7/12   
----
這兩週再學習yii框架，如果有人有興趣的話可以到下面的網址觀看  
yii  
https://www.yiiframework.com/  
***
>這是一個php的mvc框架，mvc的基本概念就不提了相信大家都懂  
一開始yii框架會先執行web/index來執行  
yii當中控制部份會要求檔案名稱以Controller為結尾  
如果是localhost的話，理論上URL會是  
localhost/site/index  
再這裡程式是這樣運作的  
首先框架先執行起來，然後去找到Controllers/SiteController.php  
再找到Controller當中的actionIndex去渲染整個view  
所以URL的當中site指的是SiteController，index指的是actionIndex  
而以上這些又會指向到view/site/index當中  
***
>當你在SiteController中新增的一個新的action，如`actionText()`時  
導向這個action的URL應該為  
localhost/site/test  
請注意雖然function 當中的Test是大寫，在URL中還是要用小寫  
如果是駝峰式寫法，如`actionTextSummit()`時  
導向這個action的URL應該為  
localhost/site/test-summit  
***
>view中的資料夾最好也應到Controller的名稱  
在`return $this->render('index')`的時候才不容易出錯  
***
心得：  
上面這些東西小弟真的是撞牆撞得頭破血流才摸懂這些東西，一路上該踩的坑都沒有放過docker、JS、DB、有些是我的鍋有的不是  
如果有哪裡理解錯誤還請幫忙指正，目前都還在學習的階段也希望各路朋友一起學習討論。  
PS.其實很多學校老師沒有教你的事~~都在蹺掉的課講~~真的是在外面跟別人一起coding或是上班之後才會學到，如果有機會真的可以在學校期間參與一些專案。  
像是多按`Reform code`(雖然現在做的專案按了會出事)  
很多變數名稱、副程式名稱的命名要足夠精確就算長一點也要寫好(含著眼淚看著前輩幫我code review)  
