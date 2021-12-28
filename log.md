# 100 Days Of Code - Log

### Day 0: 2021-12-19

**Today's Progress**: 在家裡的mac mini裝好Eclipse IDE，建立一個managed C project（沒有產生Makefile，由IDE管理建置動作）。一開始在IDE裡執行build時會出現「make: Nothing to be done for all」的警告，參[make: Nothing to be done for ‘all’ – Eclipse Error Solve](https://www.fayewilliams.com/2015/02/24/make-nothing-to-be-done-for-all-eclipse-error-solved/)，把executable name改個名字就好了（奇！）。本日開始照C How to program書中的Listing 7-24開始coding練習：#include與#define這兩個preprocessor命令的用法、字串陣列的宣告與初始化、單雙引號用於字元和字串、time／rand／srand的用法

**Thoughts:** printf中的列印格式化還沒弄熟.

**Link to work:** [7_24.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/7_24.c)

### Day 1: 2021-12-20

**Today's Progress**: 完成7-24程式，學到快速初始化int array值的方式、使用do…while。明天要正式啟動100DaysOfCode活動，並且會fork他們提供的一個github repo，之後會移往那裡做活動記錄。

**Thoughts**:

**Link(s) to work**: [7_24.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/7_24.c)


### Day 2: 2021-12-21

**Today's Progress**: 完成7-26程式，學到用C寫[泡沫排序](https://zh.wikipedia.org/wiki/%E5%86%92%E6%B3%A1%E6%8E%92%E5%BA%8F)。

**Thoughts** 發現自己對算法真的不熟。用指標做兩個值的交換也寫得卡卡，函式指標第一次用，對它的語法也挺陌生。

**Link(s) to work** [7_26.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/7_26.c)

### Day 3: 2021-12-22
**Today's Progress**: 閱讀Summary of Chapter 7 「C Pointers」，回答自我測驗，把測驗7.3寫成程式。

**Thoughts** 唸書是一回事，實際寫code是另外一回事，還沒有到非常流利的程度，寫code時都要先想一想、回憶一下語法。

**Link(s) to work** [ex_7_3.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/ex_7_3.c)

### Day 4: 2021-12-23
**Today's Progress**: 閱讀Chapter 8 「C Characters and String」從8.1到8.5，並把8.5的內容用程式實做，學到了ctype.h裡的幾個function，把string轉成double或long的functions，如何使用fgets、getchar從命令列輸入讀取資料。

**Thoughts** 有關字元與字串的函式非常多，沒辦法一次就全部弄熟，需要時間多練習。

**Link(s) to work** [sec_8_5.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/sec_8_5.c)

### Day 5: 2021-12-25
**Today's Progress**: 讀完Chapter 8 「C Characters and String」，學到string.h裡例如strcpy、strcat的函式。一些對string做搜尋的函式不太容易理解，像是strpbrk就很難從函式名稱看出它的用途。
這章雖然在講字元與字串，但8.9節郤在談對memory(也就是對變數)做類似處理（像是memcpy）的一些函式。
回答幾個self-review questions，挑了習題8.11來實作。

**Thoughts** 還是很不習慣用陣列和指標來操作字串，發明C的人當年幹麼不真的弄個字串資料型態出來？

**Link(s) to work** [ex_8_11.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/ex_8_11.c)

### Day 6: 2021-12-27
**Today's Progress**: 讀Chapter 9 「C Formatted Input/Output」中printf的部份。今天好睏，
就沒有寫code練習了，這些東西在Java、Python裡也有，但或許有細微出入吧？這本書把格式化字串分成conversion
specifier（熟悉的d、s、f等）、flags（如用-做向左對齊）、field width（ex：%8d）、precision（
ex：%.3f）與literal characters（ex：\t、\n），這樣分類好有比較好理解。

**Thoughts** 記得住而且會用的，似乎永遠只有那幾個。

### Day 7: 2021-12-28
**Today's Progress**: 讀完Chapter 9 「C Formatted Input/Output」，其實只是scanf的用法，
如何用它讀入數字、字元、字串值。由於今天休假去禮納里走走，回來沒有寫code練習的時間，純粹只是讀書，但最後有打開IDE驗證一下讀入兩個整數的反應。在scanf中搭配field width會有不同的效果：scanf("%2d%d",a,b)，輸入123_456（_代表一個space），結果a=12,b=3。此外，printf中的%i就是列印一個有號十進位整數，但scanf中的%i，可用來讀入十進位、八進位（ex：070）、十六進位（ex：0x70）整數。 
