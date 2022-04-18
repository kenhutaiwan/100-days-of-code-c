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

### Day 8: 2021-12-29
**Today's Progress**: 閱讀Chapter 9 「C Structures」，從10.1到10.5。撰寫程式練習如何定
義一個structure、建立一個structure變數並賦值、使用dot operator與arrow operator來對structure
member取值。

**Thoughts** structure在C裡蠻重要的，因為它不是物件導向語言，所以藉由structure來把相關變數
集中在一處，以提供基本的模型定義功能。

**Link(s) to work** [10_2.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/10_2.c)

### Day 9: 2022-01-16
**Today's Progress**: 因為新年與預備1/12在PMI高雄分會的分享，中斷了兩個星期。今天先複習
Chapter 9 「C Structures」，從10.1到10.7的內容，然後以P444-445 Listing 10.3的洗牌程式
為練習對象，完成自己的coding實做。

**Thoughts** 隔一段時間後又生疏了一些，過程中卡在C裡要如何宣告陣列（又回到Java的舊習慣，想去new
個array）、如何取亂數，連C的null要怎麼寫都忘了。

**Link(s) to work** [10_3.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/10_3.c)

### Day 10: 2022-01-17
**Today's Progress**: 閱讀10.9 Bitwise operator，講到C語言中的位元運算。10.10 Bit Fields
是個有趣的東西，它可以用在struct或union裡，並不是說這種field只能有一個bit，而是可以對int或
unsigned int的field指定用幾個bit（甚至是0個）來儲存。10.11 Enumeration Constants，和Java
裡的enum像，又不完全像。10.12 Anonymous Structures and Unions，一開始書上說struct裡不可
以有別的struct，但自C11起有例外：struct裡可以有匿名struct。

**Thoughts** 對enum做for loop的寫法一開始用錯，後來想想，要在java裡做這件事，其實類似。

**Link(s) to work** [10_7.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/10_7.c)、[10_18.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/10_18.c)

### Day 11: 2022-01-18
**Today's Progress**: 閱讀12.1到12.4，介紹如何在C語言裡用self-referenced struct來實做
linked list。今天的實做只做到insert和print，delete還沒有做。其實可以看看Java裡的LinkedList
提供哪些method，把它們在C裡實做出來，也算是蠻好的練習。

**Thoughts** 在Java裡簡簡單單地new個LinkedList或ArrayList來用，沒想到在C裡要自己來寫。
難處仍然在指標，在書本範例裡，為了pass by reference，用來指標的指標，這招對目前的自己，仍然算
是奧秘啊！

**Link(s) to work** [12_3.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/12_3.c)

### Day 12: 2022-01-20
**Today's Progress**: 繼續之前的linked list實做，加上delete。

**Thoughts** 函式呼叫有呼叫方（caller）與被呼叫方（callee），要在caller接收callee造成的
變化，一種方法是接收回傳值，另一種則是用pass by reference。今天在做delete時嘗試了這兩種，後
者需要傳入「pointer of pointer」， 在函式裡處理這種東西時得時時提醒自己現在處理的到底是pointer
還是pointer of pointer，決定要用address operator還是indirection operator，腦袋快打結了。

**Link(s) to work** [12_3.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/12_3.c)

### Day 13: 2022-01-21
**Today's Progress**: 參考書上的fig 12.8，實做一個簡單的stack結構(FIFO)。

**Thoughts** 有了linked list的實做經驗，這回再度使用pointer to pointer來做事，感覺順利多了。

**Link(s) to work** [12_8.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/12_8.c)

### Day 14: 2022-01-24
**Today's Progress**: 參考書上的fig 12.13，實做一個簡單的queue結構(FIFO)。

**Thoughts** 一開始沒辨識出Queue需要用到兩個指標，分別指向頭端和尾端。

**Link(s) to work** [12_13.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/12_13.c)


### Day 15: 2022-01-25
**Today's Progress**: 參考書上的fig 12.19，實做一個二元搜尋樹：值不重複，每個節點只有左和右
兩個子節點，左節點一定<父節點；右節點一定>父節點。

**Thoughts** 不寫不知道，原來組建二元樹以及用前、中、後序遍歷樹，都充份利用到遞迴。對於遞迴在
建樹與遍歷時的處理過程其實沒真的搞懂，主要還是參考了書上的範例程式來把它做出來，後續還要再加強觀
念。

**Link(s) to work** [12_19.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/12_19.c)

### Day 16: 2022-01-28
**Today's Progress**: 閱讀第十三章：C preprocessor。之前曾在一些程式裡看過它們，有些preprocessor
當時並不瞭解用意與用法，原來可以定義巨集（macro）、可以做assert、改變輸出顯示時的行號等等。今天
沒有做任何程式實作，先讓自己對這些preprocessor有個印象，之後突然想到有什麼應用的機會時，再回來
查閱。本章共提到以下這些preprocessor：
- #include
- #define：用來定義符式常數（symbolic constant）或巨集（macro）
- #if、#endif、#ifdef、#ifndef、#elif、#else
- #error
- #pragma
- \# and ## operator
- #line
- 幾個預定義symbolic constant，ex：_FILE_
- assert（它其實是個定義在assert.h的macro）

### Day 17: 2022-01-29
**Today's Progress**: 今天開始學習CMake。之前在做影像辨識、IEC-61850時都遇見過它，當時只
覺得很難理解，今天則先看過二、三篇快速上手文，用目前在做的C語言練習專案來嘗試，發現其實也並不是
真的那麼難。同時也在notion上建立了cmake的筆記頁面。

**Thoughts** 在Mac上也可以直接使用make，要用到cmake的時機目前剩下要在windows上做編繹，或是
用來產生給visual studio或xcode用的project file。但我想把它學好一點，多少是有用的，或許回去
用clion，就不會那麼恐慌了。

### Day 18: 2022-02-08
**Today's Progress**: 過完年回高雄，昨天重拾C How to program這本書，在chapter 5 C Functions
這章的exercise中挑了5-36 Tower of Hanoi來做。知道要用遞迴，但開始後就寫不下去，難以推導出
遞迴的寫法。看了兩篇介紹遞迴的文章，今天上班時用紙筆先做一次推導，才試出來。回家後又挑了5-35，寫
個非遞迴（改用迴圈）的Fibonacci series，也花了點時間。

**Thoughts** [为什么你学不会递归？告别递归，谈谈我的一些经验](https://zhuanlan.zhihu.com/p/59389994)，作者整理了自己如何理解並推導遞迴寫作的想法，從回應來看，大多數人贊同，但也有少數人不
做此想。但作者提出的三步驟，我覺得是有幫助。

**Link(s) to work** [ex_5_35.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/ex_5_35.c)、[ex_5_36.c](https://github.com/kenhutaiwan/learning-practice/blob/main/c/c_how_to_program/src/ex_5_36.c)

### Day 21: 2022-02-22
**Today's Progress**: 利用CMake官網的[教學](https://cmake.org/cmake/help/v3.23/guide/tutorial/A%20Basic%20Starting%20Point.html)並clone他們的source code來做CMake的練習。
可以在CMakeLists.txt裡定義應用程式版本，然後生成header供程式include。

```
target_include_directories(Tutorial PUBLIC
                           "${PROJECT_BINARY_DIR}"
                           )
```

這段目前不太理解，但${PROJECT_BINARY_DIR}似乎對應到我所在的執行目錄（Step1_build），因生成的
TutorialConfig.h產生於此。

原來可以用`cmake --build .`取代直接執行產生的Makefile，要指定C++語言特定版本，使用：

```
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)
```

教學的第二步（Step 2）講到如何加入一個函式庫（由一個.cxx、一個.h檔組成），這應可類比到我在C專
案自己寫的.c、.h。要做這件事，用到add_subdirectory、target_link_libraries、target_include_directories等指令，也示範了如何用option指令來建立一個ON／OFF的選擇器：`option(USE_MYMATH "Use tutorial provided math implementation" ON)`，
在程式裡透過這個選擇器的ON／OF來決定要使用哪一個庫：

```
#ifdef USE_MYMATH
  const double outputValue = mysqrt(inputValue);
#else
  const double outputValue = sqrt(inputValue);
#endif
```

若指定為ON：`cmake ../Step2 -DUSE_MYMATH=ON`，產生的TutorialConfig.h裡，會帶有一行：`#define USE_MYMATH`

**Thoughts** 一直很想把CMake學起來，過去由於教學用的是C++的例子，一直有點排斥，後來才想通：
從教學可以看到如何一步步用CMake建立專案建置方案，自己再想辦法套用到C專案上就好了。

### Day 22: 2022-02-24
**Today's Progress**: 繼續 CMake官網的[教學](https://cmake.org/cmake/help/v3.23/guide/tutorial/A%20Basic%20Starting%20Point.html)的Step3、Step4。使用target_include_directories與
INTERFACE關鍵字來定義使用需求（usage requirement），CMake的PUBLIC、PRIVATE、INTERFACE
不好理解，有人寫了篇心得：[CMake: Public VS Private VS Interfac](https://leimao.github.io/blog/CMake-Public-Private-Interface/)，用物件繼承系統的這類修飾子去想，比較容易明白。

```
target_include_directories(MathFunctions
          INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}
          )
```
Step4則介紹怎麼用CMake提供install與test兩種建置目標（goal），測試結果，cmake的install要
在源目錄（ie：CMake/Help/guide/tutorial/Step4）才有用，在另建的build目錄執行會失敗（但用make install是OK的）：

```
cmake --build .
cmake --install .
```
但若像上頭那樣不用--prefix指定安裝目錄，預設會安裝到以下系統路徑：

> -- Install configuration: ""
-- Installing: /usr/local/bin/Tutorial
-- Installing: /usr/local/include/TutorialConfig.h
-- Installing: /usr/local/lib/libMathFunctions.a
-- Installing: /usr/local/include/MathFunctions.h


**Thoughts** CMake的tutorial真的不好讀、不好理解，應該一步步仔細研究它，查清楚每個指令的用
途，然後特別為此寫筆記做學習記錄。另外，在網路上找到的CMake Cookbook看來比較容易讀喔。

### Day 23: 2022-03-23
**Today's Progress**: 不得了，居然停了一個月！繼續 CMake官網的[教學](https://cmake.org/cmake/help/v3.23/guide/tutorial/A%20Basic%20Starting%20Point.html)的Step5。使用check_symbol_exists模組來檢查系統上有沒有需要的function存在，若有，則在原始碼中使用它。至於如何讓程式原始碼知道檢
查結果，作法是先使用來建立所謂的compilation definition：`target_compile_definitions(MathFunctionsPRIVATE "HAVE_LOG" "HAVE_EXP")` ，然後再於原始碼中用`#if defined(HAVE_LOG) && defined(HAVE_EXP)`來取得檢查結果。

**Thoughts** 如果我要開發的C程式對平台有相依性，今天學到的這一招應該可以派上用場。

### Day 24: 2022-03-24
**Today's Progress**: 繼續CMake教學的Step6。使用add_custom_command來增加一個自定義命令
(command),在編繹過程中藉由這個命令的執行來産生一個檔案,這個檔案也會被用在程式的運算中,因為那個
自定義命令所對應的C++程式産生的是一個header file,被include後會使用其中旳一個double array.

**Thoughts** 有時在軟體建置的過桯中會需要産生一些中間檔供定用途使用,此時就能派上用場.

### Day 25: 2022-03-26
**Today's Progress**: 先暫停CMake的學習，因為一直到現在，對它還沒有太多感覺，或許再找一、兩
篇寫得不錯的教學文來加深體會一下。從今日開始改以從借閱的《C/C++演算法》（by 秦姣華、向旭宇）的學
習為主，先照2.3的內容寫個順序表（sequential list），它的底層還是陣列、結構（struct）與指標，
正好也用此機會複習C的基礎。過程中發現自己又忘了不少，像是在C裡不能用==比較兩字串、以char陣列儲存
字串的賦值方式等。

**Thoughts** 寫完了想一想，這個順序表不就是Java的ArrayList與Python的List嗎？至於不用陣列
而用順序表，我想是因為透過表的一些function可以有更好的操作性。

### Day 26: 2022-04-14
**Today's Progress**: 這陣子天天忙著追EMS技轉的課程復習進度，撥不出時間來進行C的學習。這兩
天按照《C/C++演算法》2.8節談的圖結構的內容，實作了一個簡單的程式，可用來建立一個圖結構，然後
遍歷、列印它。

**Thoughts** 那本書不是專門講資料結構的書，對圖結構只是舉例說明，相信之後有時間專心研究資料
結構主題時，對不同的圖結構與遍歷方式應該有更多東西要學。

### Day 27: 2022-04-18
**Today's Progress**: 按照《C/C++演算法》第三章的內容，練習三個程式，分別是求雞兔同籠問題的
窮舉法、求Fibonacci數的遞推法以及求階乘的遞迴法。原本做了第四個練習：用分治法（divide and
conquer）找假硬幣，接近完成，但目前設計不容易顯示最後找到的是第幾枚硬幣。

**Thoughts** 今天的題目，除了分治法之外，倒還蠻簡單的。分治法遇到盲點：最後怎麼知道是哪一枚硬
幣？書上的做法是一堆硬幣的Low與High：低高位位址，而我是用陣列大小當傳遞參數，所以才遇到困難。
