Common variables in spatial analysis are divided into two types. One type is known as regional attribute variables, which represent the unique attributes of each region. Examples include socio-economic background variables or the distances calculated to the target in the previous weeks, including the number of targets. These are all considered regional attribute variables. The second type of variable is known as contextual variables, which are unrelated to regional attributes. For example, the performance (variable values) of neighboring regions, which is generally represented as WY. W represents the adjacency matrix, and Y represents the variable.

The W adjacency matrix is an nXn matrix, where the value is 1 if two regions are adjacent and 0 otherwise. The adjacency relationship is defined by the researcher; neighboring regions are considered neighbors. Neighbors can be defined as regions sharing a boundary or as geographical units within a certain distance. There is no fixed standard for defining neighbors; the basic principle is that neighbors are those with potential mutual influence. Thus, the meaning of neighbors in agricultural societies differs from that in industrial societies.

W is a 0-1 matrix, and after row normalization, the sum of each row's values is 1, effectively defining the weights of neighbors. The weights of neighbors can vary as long as the sum is 1.

WY essentially represents the multiplication of the W and Y matrices. The former is an nXn matrix, while the latter is an nX1 matrix, resulting in WY being an nX1 matrix. Its physical meaning is the performance of the neighbors.

WY represents the performance of neighbors. If all neighbors have equal importance, the performance of the neighbors is the simple average of the neighbors' variable values. If the importance of neighbors varies, the result is a weighted average based on different weights.

The focus of this project is to generate the adjacency matrix and calculate the neighboring performance. The correlation between one's own performance and that of neighboring regions can be analyzed and tested. If the null hypothesis is rejected, it indicates that one's own performance and the performance of neighbors are not independent but mutually influential. This is known as spatial autocorrelation.


空間分析中常見的變數可分為兩類，一類稱為地區屬性變數，它代表各地區特有的屬性。例如：社會經濟背景變數，或前幾週計算的與目標點的距離，以及包含目標點的個數等，這些都屬於地區屬性變數。另一類變數稱為脈絡變數，它與地區屬性無關。例如鄰近地區的表現（變數值），我們一般用WY表示。其中，W代表鄰近矩陣，Y代表變數。

W鄰近矩陣是一個nXn的矩陣，若兩地區存在鄰近關係，其值為1，否則為0。鄰近關係由研究者自行定義，有鄰近關係的地區即為鄰居。可以將周邊領土相連的地區定義為鄰居，也可以將一定距離內的地理單元定義為鄰居。鄰居的定義沒有固定標準，基本原則是存在相互影響的可能性才算是鄰居。因此，農業社會中的鄰居與工業社會中的鄰居意義自然不同。

W是一個0、1矩陣，經過行標準化後，每行的值總和為1，即為鄰居的權重。鄰居的權重大小不一，只要總和為1即可。

WY的意義其實就是W與Y兩個矩陣的相乘，前者是nXn的矩陣，後者是nX1的矩陣，WY則是nX1的矩陣，其物理意義即為鄰居的表現。

WY代表鄰居的表現，如果所有鄰居的重要性相同，則鄰居的表現為鄰居變數值的簡單平均。如果鄰居的重要性不同，則依據不同的權重進行加權，其結果即為加權平均。

本專案重點在於產生鄰近矩陣以及計算鄰近地區的表現。可以對自己的表現與鄰近地區的表現進行相關分析及檢定。如果拒絕虛無假設，表示自己的表現與鄰居的表現並非獨立，而是相互影響，這稱為空間自相關。
