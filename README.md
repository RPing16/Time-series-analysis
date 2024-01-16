# Time series analysis
1.  **敘述統計分析**
2.  **計算累計報酬率**
3.  **改變時間單位**
4.  **時間窗口**
5.  **均線和黃金(死亡)交叉**
6.  **迴歸分析**
7.  **相關係數時間變化趨勢**
## code重點說明
1.  **計算累計報酬率**
- 使用cumsum().apply(np.exp)
2.  **改變時間單位**
- 使用resample('time').last()改變時間單位的數值
- 使用resample(lable)改變時間單位的index
3.  **時間窗口**
- 使用rolling(window)
4.  **均線和黃金(死亡)交叉**
- 均線 : 使用rolling(window).mean()
- 黃金(死亡)交叉 : 使用np.where()
5.  **回歸分析**
- 使用np.polyfit(x,y) fit Y = b0 + b1X
6.  **相關係數時間變化趨勢**
- 使用rolling(window).corr()
