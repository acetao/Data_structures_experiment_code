### 用栈求解迷宫问题的所有路径以及最短路径
# 基本思路：
（1）将迷宫存在二维数组中，0表示可走，1表示不可走。在迷宫数组四周加一堵“围墙”，表示其不可走。  
（2）定义一个Box类表示所走方格，可走时压入栈，栈用vector库实现。  
（3）按上右下左的顺序为方位编号1，2，3，4，未走时候默认方位数为0。  
（4）已经走过的位置其值置1，表示不可走，回溯时撤销，使其重新可走。
