# 軟體工程FINALPROJECT

* ### 系統架構圖
> 當使用者想要知道如何解題時，點擊螢幕選擇語音或是鏡頭辨識，機器人就會依據使用者要求，透過鏡頭或語音讀取題目，接著程式就會根據題目，透過程式運算得出解答與步驟，將解題步驟透過螢幕與語音傳遞給使用者。而後透過鏡頭擷取使用者作答過程，一步步判斷使用者作答狀況，達到學習解答的目的。
家長透過WIFI連線的方式，連上機器人的前鏡頭，觀看學生的即時影像。

![image](https://user-images.githubusercontent.com/92836676/147932473-8b8a6962-f701-4e64-a929-75cd7fae273b.png)

* ### 鏡頭識別
圖像識別系統是使用OpenCV中的OCR(光學字元辨識)，我們引用的是Pytesseract，只要使用者將圖片拍照匯入程式中他就能將圖片轉成文字檔，也可以將使用者書寫的文字識別進電腦裡，這技術精準度很高也支持多個語言的轉換，目前此軟體是由Google進行維護。

![image](https://user-images.githubusercontent.com/92836676/147932442-ef2af85e-bfd6-4710-96f3-dc13e11d215c.png)

* ### 語音識別
語音識別系統是使用Google API，雖然它的音檔較大，而且需要連接網路才可使用，不過網路越快，辨識的速度也就越快，再加上它可以偵測多國語言而且準確率很高，不太會造成使用者的困擾。

![image](https://user-images.githubusercontent.com/92836676/148095905-32b340dd-df0e-42b0-bbc4-b4b3f09bfb0d.png)
![image](https://user-images.githubusercontent.com/92835373/148686641-b51ccab9-3ecd-4ea8-80df-c53b7c4364f5.png)

* ### 家長監控
使用Python加上OpenCV的功能，來使用家教機器人上的鏡頭，以網路來連接，家長可以透過手機，及時觀察學生的狀況。

<img src="https://user-images.githubusercontent.com/92836676/147932333-2d870899-4b8c-4a86-a43b-f4a8311478f8.png"  width="500" height="400">

# 操作步驟

點擊螢幕上 **語音辨識**，當家教機器人語音讀取到題目，在程序內部轉換成文字，判斷題目後，尋找題庫或是運算來得出解答，並輸出詳解步驟，將步驟顯示於螢幕上。機器人可逐步教學，以語音以及螢幕上顯示的詳解來教學，再透過攝影機的鏡頭判斷學生作答的正確性，判斷是否正確，不對的話會反應到螢幕上，糾正後再判斷，若題目作答正確即完成。

點擊螢幕上 **鏡頭辨識**，當家教機器人鏡頭讀取到題目，在程序內部轉換成文字，判斷題目後，尋找題庫或是運算來得出解答，並輸出詳解步驟，將步驟顯示於螢幕上。機器人可逐步教學，以語音以及螢幕上顯示的詳解來教學，再透過攝影機的鏡頭判斷學生作答的正確性，判斷是否正確，不對的話會反應到螢幕上，糾正後再判斷，若題目作答正確即完成。

點選 **題庫**後，選擇出版社及年級，再依照科目去尋找，進入選定科目後，再選擇單元，即可檢視該科目題庫。

點選 **弱點加強**，進入後選擇科目，程序會生成出奇錯誤率較高之題型，產生出考試卷，題目數約有5到10題，依照其題型之題目數做增減。

若使用 **電子書** 的功能，可透過教科書商的電子書課本，使用電子書上的教學，其餘詳細功能，則配合書商提供的系統。

家長的部分，如果想查看學生的學習狀況，可透過網路連線機器人，是用手機連上鏡頭，可以及時監督學生是否用功讀書。

# 進度規劃
<img src="https://user-images.githubusercontent.com/92835373/148771475-0f598bbe-43f9-4d7c-bb7a-fbe9c9d773c2.png"  width="600" height="400">
---------------------------------------
# 參考文獻
* mathAI：https://github.com/Roujack/mathAI
* OpenCV：https://medium.com/ching-i/python-opencv-%E8%AE%80%E5%8F%96%E9%A1%AF%E7%A4%BA%E5%8F%8A%E5%84%B2%E5%AD%98%E5%BD%B1%E5%83%8F-%E5%BD%B1%E7%89%87-ee3701c454da
* COR：https://dotblogs.com.tw/RYNote/2021/01/14/105447
* Google API 語音辨識：https://www.oxxostudio.tw/articles/201509/web-speech-api.html
* ROYBI機器人：https://www.epochtimes.com/b5/21/6/20/n13035239.htm
* Photomath：https://agirls.aotter.net/post/52065
* Microsoft Math Solver：https://math.microsoft.com/zh
* Mathway：https://www.pkstep.com/archives/22122
* NUWA科技：https://www.nuwarobotics.com/zh-hant/
* Kebbi Air S：https://www.esentra.com.tw/product/kebbi-air-s/
---------------------------------------
