這是以爬梯子的原型製作的遊戲，但是一般的爬梯子是隨機產生籤紙，沒有辦法和使用者互動。所以我製作一個實用且能夠讓所有人有參與感的抽籤網頁。

起始頁面：
  底圖使用illustrator製作，大概介紹這個遊戲的起源和提供不同語言的連結
  
遊戲頁面：（不同語言內容相同）：
  所有視覺圖像皆是使用illustrator製作，包括底圖、說明欄、主題籤（右下方可以選擇主題）
  籤圖本體：使用table製作，由窄欄（垂直粉紅）和寬欄（可選擇水平線）相間
    css:色調、大小、位置、hover
    js：計算和特效
      初始設定按鈕及對應的函式
    演算方式（js）：
      使用兩個陣列，其一用來計算按鈕狀態(True/False),以True表示按鈕可被選按，False表示按鈕被鎖住無法選按，且相鄰兩按鈕不可被同時選擇，故選擇是相鄰       的按牛狀態也會改為False(if函式判斷按鈕可否被選按)；另一個陣列用來表示已選擇的狀態，一樣以True/False表示，但相鄰的按鈕不會被改變以便計算。
      結果預設為一陣列（及沒有任何畫記時的結果），判斷沒一列兩旁如果遇到False就要向左或右的選項移動。
  
  確認人數：
      一開始填入人數，用js讀入輸入欄資訊後鎖住超出人數的按鈕（改為False)
  
 
