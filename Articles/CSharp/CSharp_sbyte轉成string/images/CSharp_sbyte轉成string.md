# C# sbyte 陣列轉換為 string

最近在使用第三方 API 時，因為第三方是使用 Visual C++ 開發的，但是我們平常所開發的軟體是 C#，因此需要有一個將 C++ 轉成 C# 的中介類別，方便我們直接呼叫；但在取得字串的過程中碰到一些問題
我們要在 C# 呼叫他的函式庫使用

最近在撰寫 NCLinker 檔案傳輸發現一個蠻方便的東西，在這邊分享給大家。大家都知道三菱函式庫是使用 C++ 開發的，因此我們要呼叫使用他的函式庫必須使用 C++ 做呼叫，但是我們平常所開發的軟體是使用C#，所以還有一個將C++轉換成C#的中介類別，方便直接就可以用C# 呼叫函式，但是在將 VC++ 資料拿回來時，通常都需要做一些處理 C# 與 VC++ 之間才有辦法共享資料，本篇主要想要介紹其中一個檔案傳輸會使用到的方法，將 VC++ 那端所得到的 sbyte 轉換成 C# 的 string。

