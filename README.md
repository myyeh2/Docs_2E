<!--     C:\2302\github\Docs_2E       -->

#  
<!--                 
# \[{  \color{Fuchsia}精\;銳\; \color{Purple}矩\;陣\;  \color{Red}計\;算\; \color{Green} 求\;解\;器  }\] 
-->  

 ![](Images/11-10-01.png) 

<!--         
#### \[{  \color{Fuchsia} 【 \color{Green}  Sharp \; Matrix \; Solver \;  \color{Brown} \iff  \;  \color{Red} S\;M\;S】 }\]  
-->  
![](Images/11-10-02.png)  

##  

<!--   
###### \[{ \color{Red} {從\;微\; {\color{Brown}分\; {\color{Fuchsia}方\; {程\; \color{Green} {式\; { \color{Blue} 起\; \quad \Rightarrow}  }  }  }  }  }  }\] 
### \[{  \color{Red} 經\;由\;系\;統\; \color{Blue}矩\; 陣\quad \color{Green} \Rightarrow }\] 
# \[{  \color{Brown} 求\;得\; \color{Red}系\;統\; \color{Green}響\;應\;值\quad \color{Brown} \oplus   }\]
-->
######  

![](Images/06-27-01.png)  

<!--   
# \[{  \color{Purple}Computational \quad \color{Fuchsia}Matrix  }\] 
-->
![](Images/06-27-02.png)

<!--    
######  \[{ \color{Blue} for }\]
-->
![](Images/06-27-06.png)  


<!--     
### \[{  \color{Green} Signals \; \color{Fuchsia} and \; \color{Blue} Systems \; \color{Brown},   }\]
### \[{   \color{Red} Control \; \color{Green} Systems \; \color{Brown} ,  }\]
### \[{   \color{Red} 結 \; 構 \; \color{Blue} 動 \; 力 \;  學 \; \color{Brown},  }\]
### \[{   \color{Red} 動 \; 態 \; \color{Fuchsia} 系 \; 統 \; .\;.\;. \color{Brown} \; 等 \; 等  }\]
-->
![](Images/06-27-03.png)  

<!--      
### \[{  \color{Green} 參\;見\; \color{Gold}本\;儲\;存\;庫\; \color{Blue} 的\;程\;式\;碼 \color{Brown}。 }\]
##  
## \[{  \color{Olive} AI人工智慧 \color{Coral} 與 \color{#E9EAEC} 物理、機電實驗的\color{#FFDF00}響應  }\]  
-->
![](Images/06-27-04.png)  


<!--       
######  \[{  \color{Cyan}使\;用\;以   }\]  
-->
![](Images/06-27-07.png)  


<!--    
### \[{  \color{Teal} System-Driven(系統驅動)   }\]  
### \[{  \color{Maroon} Engineering \; \color{Chocolate} and \; \color{Khaki} Science \;  \color{Indigo} Computation  }\]  
### \[{  \color{Magenta} 工程和科學 \color{Chocolate}計算   }\]  
-->
![](Images/06-27-05.png)  

###  

<!--    
####  \[{  \color{Teal} *\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;* }\]  
-->
![](Images/06-27-08.png)  

##

##### **看了Youtube【科學史沙龍】**  

### [蔡教授的演講，虛幻乎？真實乎？-談虛數的幻與真。](https://www.youtube.com/watch?v=n9cMg0e8KBw)  

##### **我非常同意這句話，在數學世界裡，有古典名言【連結實數世界裡兩個真理的最短路徑，是通過虛數】，並非科幻之談。但不知是否改爲【實數的數值計算過程中，若無法使用實數值來表示數值，必須改爲複數值來表達，再繼續使用複數矩陣計算，複數矩陣計算的最後結果，仍然是複數矩陣，但我發現此複數矩陣的虛數值為零，故可去掉零的虛數值，最後又回到實數矩陣的世界，故我的結論是【實數值是真實的數值，複數值僅是中間必要的計算過程而已，最後計算結果都應該回到實數的真實世界中】。這是我使用C#程式語言撰寫矩陣計算，以常微分方程式的齊次解，求得複數特徵值與複數特徵向量，無意中發現的結果，連我自己也表示驚訝！但我不知道是否正確？也需要更多的同好、專家、學者的評論，故在此請益、多多指教。**  

##### **直接使用單一個的複數做計算，我個人認爲可能有問題？但大家都是這樣作。僅單單一個複數值，我們並不知道是代表什麽意思。應該是由微分方程式，得到系統矩陣，再得到複數的特徵值與特徵向量矩陣，最後求得系統的響應值。一般訊號與系統的書，都是直接使用複數，虛數值就是頻率，作所謂的Fourier、Laplace和Z轉換等等。空間維度(Space Dimension)僅有一個自由度(Degree of Freedon)，狀態維度(State Dimension)可以有多個自由度，似乎較容易求解，但若是空間與狀態維度有多個自由度時，需要使用矩陣的數學模型計算，就如上所述的由微分方程式求得到系統矩陣，再求得整個系統隨著時間(t)變化的響應值，可參見本儲存庫(Repository)相關的程式碼。**  

##### **我這樣的發現，是依據矩陣的計算理論，使用C#程式語言撰寫矩陣的計算所發現的結果。譬如求解多項式的根，將多項式轉爲矩陣的形式，發現多項式的根，就是矩陣的特徵值，在計算的過程中，無法使用實數求得多項式的根，必需轉爲複數才可求得。另外對於【非對稱實數矩陣】的特徵值和特徵向量，也是無法使用實數值求得，必需轉爲為複數，使用複數矩陣的計算，計算包含複數矩陣的加、減、乘、除、轉置、求逆、合並等等，雖然最後複數矩陣的計算結果也是複數矩陣，我也發現該複數矩陣的虛數值為零，即複數矩陣可轉爲實數的矩陣，計算的最後結果又回到實數的矩陣，回到實數的真實世界中，不再包含虛數值。故【複數矩陣實際的計算，並不是一般純理論的推導】，這個部分即使是數學家可能也無法想像、或是無法做到的事情，以至對於虛數值產生困惑。**  

##### **我將研究的結果，包含動態系統公式的推導、C#程式的撰寫，並發佈於Github網站上。**

## [矩 陣 計 算 求 解 器](https://github.com/myyeh2/)  

#### ***在網路上，常常有人提到矩陣的對角線化，但我不知是否有人實際以程式碼去實作，對於【實數正方形非對稱矩陣】的對角化，實際上是永遠無法產生上三角型矩陣【Upper Triangular Diagonal Matrix】，這時產生的矩陣稱為【Qusi-Sub-Diagonal Matrix】，這是非常關鍵的重要型態矩陣，Qusi-Sub-Diagonal Matrix暫時稱爲【Ye Matrix，葉氏矩陣 】，我這樣稱呼的主要的原因是，我並未發現有人談到這種矩陣(若有時，本人表示歉意！也敬請Email給我)，依據維基百科之解釋就是Reduced Upper Hessenberg Matrix，由此矩陣就可以產生【複數的特徵值矩陣D】，再由複數特徵值矩陣D，推導出複數的特徵向量矩陣Q，他們的關係是【A * Q = Q * D => A = Q * D * Qi】, Qi是Q矩陣的逆矩陣，即使Det(A) = 0，但Q矩陣也永遠不為零。另外值得一提的是，若系統矩陣A為正方形實數對稱矩陣，則Q和D都是實數，且Qi = Qt，即A= Q * D * Qt。總而言之實數是複數的subset，即複數的Scope大於等於實數的Scope。***  

#### ***數值求解特徵值和特徵向量，與矩陣計算相關的兩本數學聖經書，第一本是James Hardy Wilkinson，"The Algebraic Eiginvalue Problem"，第二本是Gene H. Golub & Charles F. Van Loan，"Matrix Computations 4th Edition，第七章Unsymmetric Eigenvalue Problems"。若熟悉SMS(精銳矩陣計算求解器)的操作，幾乎可包含上述兩本書的精要。***  

##  

##### **對於實數正方形非對稱矩陣，如何求得[Ye Matrix]，可使用Iteration QR Method。但何謂[Ye Matrix]：即Sub-sub-Diagonal 本身和以下的元素均爲零，也就是Upper Hessenberg Matrix，而Sub-Diagonal的元素由第0元素開始，(1). 若為零時，則OK繼續前進至下一個。(2). 若不為零時，則下一個元素，如果為零，OK繼續前進至下一個，若元素不爲零時，則NG不是【Ye Matrix】，3. 相同的步驟繼續直執行，到Sub-Diagonal最後一個元素結束，如果均符合以上的規定，則OK為【Ye Matrix】，否則不是【Ye Matrix】：換言之如果第0個至最後一個Sub-Diagonal元素都符合規定，則為【Ye Matrix】，否則不是【Ye Matrix】。符合【Ye Matrix】規定者，可建構複數特徵值矩陣D和複數特徵向量矩陣Q。**  

#### ***若實數正方形對稱矩陣，求得的特徵值矩陣、和特徵向量矩陣一定是實數，也就是沒有動態的特性了。***  

##  

##### **我們常常談到特徵值與特徵向量，但好像沒有人提到？如何使用特徵值和特徵向量？他們用在什麽地方？如何使用程式碼實作求取？一般都是使用Matlab軟體求得，即使是使用Python的第三方程式庫【Extension】，求取也不是很完整。故希望本精銳矩陣計算求解器Add-On，在微軟Visual Studio的執行環境中使用，是一種方便的選擇。**

<!--    
# \[{ \color{Lavender} 在 \; Visual \; Studio \; 中\; 執\; 行 \; ! }\]
-->  
![](Images/06-27-09.png)  


<!--   
####  \[{  \color{Teal} *\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;* }\]
-->  
![](Images/06-27-08.png) 

![](Images/10-10-01.png)  

---  

# **所有的數值計算，全都以矩陣的方式進行。**  

---  

### 例如 :  5.3 + 3.7 * 6.7 / 7.8 - 1.3 = 7.1782051  

### Visual Studio 程式碼如下 :  

![](Images/07-28-01.png)  

<!--   
####  \[{  \color{Teal} *\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*  }\]  
-->  
![](Images/06-27-08.png)  

### 例如：矩陣 A, B, C, D, E 已知  

<!--  
$ A = \begin{bmatrix} 5 & -4 \\\\ 3 & -7 \end{bmatrix} \quad B = \begin{bmatrix} -5 & -9 \\\\ 6 & 9.89 \end{bmatrix} \quad C = \begin{bmatrix} 7 & 7 \\\\ 6 & -1 \end{bmatrix} $  
$ D = \begin{bmatrix} 5 & 8 \\\\ 5 & 4 \end{bmatrix} \quad E = \begin{bmatrix} 7.892 & 7 \\\\ 5 & -9 \end{bmatrix} \quad $  
-->
![](Images/07-31-01.png)  

### F = A + B * C / D - E 。 求矩陣 F  

### Visual Studio 程式碼如下 :  

![](Images/07-28-02.png)  

![](Images/07-28-03.png)  

---  

# **矩陣變數或運算元的表示方式**  

---  

#### **若矩陣變數的最後一個字元是【i】，表示是該矩陣的逆矩陣，即矩陣Ai為矩陣A的逆矩陣。若最後一個字元是【t】，表示該矩陣的轉置矩陣，即矩陣At為矩陣A的轉置矩陣。**  

#### **向量亦是矩陣，僅是矩陣的行(Column = 1)為1，為了方便一般以小寫表示向量，若矩陣的行大於1時，則以大寫表示。**  

#### **SMS共計有12個矩陣運算子：【+】、【-】、【*】、【/】、【==】(是否相等？)、【！=】(是否不等？)、【&】(水平合併)、【|】(垂直合併)、【^】(向量內積)、【~】(求逆)、【!】(轉置)、【+】(單位向量)。**[參見Docs_2D儲存庫](https://github.com/myyeh2/Docs_2D)  

#### ***SMS(Sharp Matrix Solver)，運算元(Operand)就是矩陣，包含向量。C#的矩陣表示就是double[,]，然後再把double[,]轉化為SMS的型態的ReMatrix或是CxMatrix。這樣的好處就是可以使用這12種的矩陣計算的運算子。***

#### **SMS提供了數百個矩陣計算的類別庫(Class Library)，譬如計算實數【非對稱系統矩陣】的特徵值和特徵向量(一般都是複數)、奇異值和奇異向量(SVD)、建構空間維度和狀態維度等多個自由度的系統矩陣A，即A是(mxr)x(mxr)的矩陣、系統響應值(System Response)的種種計算結果，A = L * U。A = Q * R。矩陣的顯示(列印)。Determinants(行列式)等等。並於後續中再介紹。**  

<!--  Title 1    -->
---  

# **矩陣方程、矩陣微分方程、和矩陣偏微分方程**

---  

#### **有限元素法、邊界元素法、結構動力系統、控制系統、訊號與系統等等，有關靜態(Static)或是動態(Dynamic)系統響應的求解，實際上就是空間(Space)和狀態(State)兩個互相垂直維度(Dimension)上，分別有m個和r個自由度的系統矩陣(mxr)X(mxr)的計算，空間指的是m個離散式的節點，而狀態指的是r階(Order)微分方程式，為連續時間的函式。[參見狀態空間State-spce Representation](https://zh.wikipedia.org/zh-tw/狀態空間)，參考陳啓宗，"Linear System Theory and Design，ISBN 978-0-1999-6454-3，Charpter 4 State-Space Solution and Realizations"，另再參考Matlab軟體等等的説明，本人認爲還是無法清楚説明，故以C#程式語言實作、測試與驗證。**  

#### **State_Space就是狀態維度和空間維度，維度就是英文的【Dimension】，林琦焜，"向量分析"乙書中稱量綱，空間維度和狀態維度互相垂直，類似互相垂直的X軸與Y軸一樣，在空間維度上有"m"個離散數值稱為有m個自由度DOF(Degree Of Freedom)，在狀態維度上有"r"個自由度，即是微分方程式的階度(Order)，狀態變數是連續時間的函數。狀態是某一節點(Node)在某一固定時間上有不同的變數，譬如同時有變位、速度、和加速度等不同的狀態變數。**

#### **狀態與空間的求解，實際上就包含有限元素法、邊界元素法、無網格法等等的演算法，這些都是理論的闡述，實際都要轉爲矩陣方程式(靜態系統)、矩陣微分方程式(動態系統)，但是矩陣偏微分方程式(動態系統)，其為連續性的空間，應轉爲有限離散的空間節點，降階成爲矩陣微分方程式。有關有限元素法的發展過程，**[參見力學學會第156期會訊](Images2/中華民國力學學會第156期會訊.pdf)  

#### **若空間維度有多個自由度m，或是m=1但狀態維度有多個自由度r時，使用矩陣的計算有必要性。另動態系統包含(大於等於)靜態系統，表示靜態系統是動態系統的一個特例。再談複數值包含(大於等於)實數值，表示實數值是複數數值的一個特例，雖然真實的世界是實數值，系統(數學模型，Mathematic Model)的輸入值和輸出值都應該是實數，但中間的求解的過程，可能須要使用複數值的計算，這是為什麽須要學習並使用程式語言實作(Implementation)，求解矩陣微分方程。**  



<!--    Title 2   -->  

---  

# **系統矩陣A**  

---  

#### **從高立圖書出版的【訊號與系統】翻譯書，第Page57【通常我們使用(系統)這兩個字，我們指的是系統的數學模型，而不是實際系統本身。若要特別指實際系統，我們將以實際系統稱之，以避免混肴。】**  

#### **如何求得系統矩陣A，可由【矩陣方程式】、【矩陣微分方程式】、或是【矩陣偏微分方程式，轉為矩陣微分方程式】，其理由是空間偏微分是連續性的空間，應轉為離散的節點，即有限的無網格節點法或是有限元素法或是邊界元素法等等，將矩陣方程或是矩陣微分方程，轉換為友矩陣(Companion Matrix)的方式。**  


<!--    Title 3     -->

---  

# **特徵值和特徵向量矩陣、奇異值和奇異向量矩陣**  

---  

#### **由特徵值和特徵向量我們可以建構系統矩陣A，再求得系統的響應值，可以參見上述的推導公式。**  

#### **由奇異值和兩個奇異向量我們可以建構系統矩陣A，但無法求得系統的實際的響應值，最多是近似值而已。即A * Q = P * D => A = P * D * Qi 。其中Q、P、和D一定是實數矩陣。如果要瞭解理由的話，必須要瞭解何謂奇異值和奇異向量的定義。**  

#### **由C#程式語言，令"A1 = At * A"，At矩陣是A矩陣的轉置矩陣，而A1矩陣一定是正方形實數對稱矩陣，而且與A矩陣不相等，(即A1和A是完全不相同的矩陣)，由A1矩陣的求得Q矩陣。再令A2 = A * At，A2矩陣也與A矩陣和A1矩陣都不相同，A2矩陣也是對稱矩陣，其所求得的特徵向量矩陣稱作P矩陣，經由A矩陣、Q矩陣和P矩陣可求得奇異值矩陣D。最後求得A * Q = P * D，即A = P * D * Qi。A矩陣是系統矩陣，Q矩陣、P矩陣是兩個不同的奇異向量矩陣，D矩陣是實數奇異值矩陣。我找到兩篇論文參考比較，另外我以C#程式碼求得奇異值矩陣、和兩個奇異向量矩陣Q和P。**  

[第一篇：陳正宗、郭柏伸、高怡娟，"可聽出鼓的形狀嗎？一對偶邊界元素分析"](https://www.math.sinica.edu.tw/media/pdf/d382/38207.pdf)  

##### **我個人淺顯的評論是，使用【奇異值】分析法，求得左右酉矩陣和奇異對角矩陣，尚有疑問之處？也希望將來有機會，能請益使用更精確的【動態複數特徵值、模態特徵向量矩陣】分析法。**  

[第二篇：國家地震工程研究中心，報告篇號：NCREE-2018-025，羅俊雄、郭采蓉、江宏偉、林云媚， "應用隨機子空間識別法於結構健康診斷：結合穩態標準與頻域分解法"](https://www.ncree.narl.org.tw/accomplishment/technicalreports/page/12034)  

#### **本文是使用"唯輸出系統識別"、"奇異譜分析法"等等，但精銳矩陣計算求解器(SMS)，是以"系統(System-Oriented)為導向的矩陣計算法"、使用"特徵譜和模態特徵向量矩陣，百分百的精準求解法"，並以C#程式語言的軟體實作，而不是純理論的闡述。**  

#### 已知系統矩陣A如下所示，求該矩陣A之特徵值矩陣、特徵向量矩陣、奇異值矩陣和兩個奇異向量矩陣，相關的程式碼和輸出結果如下  

<!--   
\[{ \color{Coral} A = \begin{bmatrix} 8.793 & 5 & 4 & -17 \\\\ 6 & -4 & -5 & 9 \\\\ 9 & 8 & 10 & -9 \\\\ -7 & -9 & 15 & 0  \end{bmatrix} }\]
-->  

![](Images2/24-08-29-01.png)  

![](Images2/24-08-29-02.png)  

![](Images2/24-08-29-03.png)  

![](Images2/24-08-29-04.png)  

![](Images2/24-08-29-05.png) 

```CSharp
using Matrix_0;

double[,] A = { {8.793, 5, 4, -17}, {6, -4, -5, 9}, 
    {9, 8, 10, -9}, {-7, -9, 15, 0} };
Console.WriteLine("列印已知矩陣A:\n{0}", new PR(A)); 

// 求特徵值矩陣和特徵向量矩陣
EIG eig = new EIG(A);
CxMatrix D = eig.CxMatrixD;
CxMatrix Q = eig.CxMatrixQ;
Console.WriteLine("特徵值矩陣:\n{0}", new PR(D));
Console.WriteLine("特徵向量矩陣:\n{0}", new PR(Q));
// 檢核矩陣D和矩陣Q是否正確？
ReMatrix Aa = (ReMatrix)(Q * D * ~Q); 
Console.WriteLine("矩陣Aa是否與矩陣A相同？:\n{0}", new PR(Aa));

// 求奇異值矩陣、奇異向量矩陣Q1和P1
SVD svd = new SVD(A); 
ReMatrix D1 = svd.MatrixD; 
ReMatrix Q1 = svd.MatrixQ;
ReMatrix P1 = svd.MatrixP; 
Console.WriteLine("奇異值矩陣:\n{0}", new PR(D1));
Console.WriteLine("奇異向量矩陣Q1:\n{0}", new PR(Q1));
Console.WriteLine("奇異向量矩陣P1:\n{0}", new PR(P1));
// 檢核矩陣D和矩陣Q是否正確？
ReMatrix Ab = P1 * D1 * ~Q1;
Console.WriteLine("矩陣Ab是否與矩陣A相同？:\n{0}", new PR(Ab));

/*以下是輸出結果 ：
列印已知矩陣A:
  8.79300     5.00000     4.00000   -17.00000
  6.00000    -4.00000    -5.00000     9.00000
  9.00000     8.00000    10.00000    -9.00000
 -7.00000    -9.00000    15.00000     0.00000
特徵值矩陣:
 12.90542 +   8.82285i,   0.00000 +   0.00000i,   0.00000 +   0.00000i,
  0.00000 +   0.00000i
  0.00000 +   0.00000i,  12.90542 -   8.82285i,   0.00000 +   0.00000i,
  0.00000 +   0.00000i
  0.00000 +   0.00000i,   0.00000 +   0.00000i,  -5.50892 +   9.66421i,
  0.00000 +   0.00000i
  0.00000 +   0.00000i,   0.00000 +   0.00000i,   0.00000 +   0.00000i,
 -5.50892 -   9.66421i
特徵向量矩陣:
  0.58429 +   0.00000i,   0.58429 +   0.00000i,   0.50777 +   0.00000i,
  0.50777 +   0.00000i
 -0.00572 -   0.09715i,  -0.00572 +   0.09715i,  -0.49147 -   0.47313i,
 -0.49147 +   0.47313i
  0.50586 -   0.44873i,   0.50586 +   0.44873i,   0.09588 +   0.06432i,
  0.09588 -   0.06432i
 -0.02400 -   0.43740i,  -0.02400 +   0.43740i,   0.30519 -   0.41268i,
  0.30519 +   0.41268i
矩陣Aa是否與矩陣A相同？:
  8.79300     5.00000     4.00000   -17.00000
  6.00000    -4.00000    -5.00000     9.00000
  9.00000     8.00000    10.00000    -9.00000
 -7.00000    -9.00000    15.00000     0.00000
奇異值矩陣:
 27.12655     0.00000     0.00000     0.00000
  0.00000    19.62379     0.00000     0.00000
  0.00000     0.00000     9.44374     0.00000
  0.00000     0.00000     0.00000     6.01582
奇異向量矩陣Q1:
  0.37740     0.46931     0.76023     0.24365
  0.36159     0.40381    -0.16468    -0.82406
  0.39110    -0.78501     0.38328    -0.28966
 -0.75754     0.02127     0.49801    -0.42151
奇異向量矩陣P1:
  0.72140     0.13473    -0.11349     0.66974
 -0.29327     0.27095     0.82445     0.40108
  0.62736    -0.02993     0.51625    -0.58224
 -0.00109    -0.95265     0.20222     0.22709
矩陣Ab是否與矩陣A相同？:
  8.79300     5.00000     4.00000   -17.00000
  6.00000    -4.00000    -5.00000     9.00000
  9.00000     8.00000    10.00000    -9.00000
 -7.00000    -9.00000    15.00000     0.00000
*/
```  

#### 已知系統矩陣A如下所示，求該矩陣A之奇異值矩陣和兩個奇異向量矩陣(不會有特徵值矩陣和特徵向量矩陣矩陣)，相關的程式碼和輸出結果如下  

<!--   
\[{ \color{Green} A = \begin{bmatrix} 9.853 & 1 \\\\ 2 & -5 \\\\ 1 & 9 \end{bmatrix} }\]
-->  

![](Images2/24-08-29-06.png)  

![](Images2/24-08-29-07.png)  

![](Images2/24-08-29-08.png)  

```C#
using Matrix_0;

double[,] A = { {9.853, 1}, {2, -5}, {1, 9} }; 
Console.WriteLine("列印已知矩陣A:\n{0}", new PR(A));  
SVD svd = new SVD(A); 
ReMatrix D = svd.MatrixD; 
ReMatrix Q = svd.MatrixQ;  
ReMatrix P = svd.MatrixP;  

Console.WriteLine($"奇異值矩陣:\n{new PR(D)}"); 
Console.WriteLine($"奇異向量矩陣Q:\n{new PR(Q)}"); 
Console.WriteLine($"奇異向量矩陣P:\n{new PR(P)}"); 

// A * Q = P * D  ==> A = P * D * Qi 
ReMatrix Aa = P * D * ~Q;  
Console.WriteLine($"矩陣Aa與矩陣A相等:\n{new PR(Aa)}");

/* 輸出執行結果：  
列印已知矩陣A:
        9.85300          1.00000
        2.00000         -5.00000
        1.00000          9.00000
奇異值矩陣:
       10.66438          0.00000
       0.00000           9.76487
        0.00000          0.00000
奇異向量矩陣Q:
        0.60513          0.79613
        0.79613         -0.60513
奇異向量矩陣P:
        0.63374          0.74135         -0.22086
       -0.25978          0.47291          0.84195
        0.72862         -0.47620          0.49229
矩陣Aa與矩陣A相等:
        9.85300          1.00000
        2.00000         -5.00000
        1.00000          9.00000
*/
```  

<!--    Title 4    -->

---  

# **系統響應、數據視覺化**  

---  






<!--   
####  \[{  \color{Teal} *\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*\;*  }\]  
-->  
![](Images/06-27-08.png)  

##  

## [精 銳 科 技【矩陣計算求解器開發】](https://www.github.com/myyeh2/App_CSharp)  

######

![](Images/name_card.png)  

##  

##  
