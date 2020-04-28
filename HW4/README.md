# Financial Engineering HW4
### [**Code**](https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Codes/Financial_Engineering_HW4.ipynb)
### [**Flow Chart**](https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Flow_Chart/Flow_Chart.jpg)
### **Learning Process**

#### 1. Risk neutral(風險中立)
風險中立的世界中假設投資人不會為了取得超額報酬承受額外的風險，他們願意只拿到無風險報酬。
由於過去的資訊已經反映在資產價格上，而未來的資產價格軌跡是未知的隨機過程，因此在一個風險中立的世界中未來的資產價格為其期望值，現值即為該期望值已無風險利率折現。    

      
期權亦可用此概念評價，首先假設以下兩個投資組合：    

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Images/未命名1.jpg" width="75%" height="75%" />    
    
由於不能套利，因此兩個投資組合擁有相同的報酬f，    

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Images/未命名2.jpg" width="50%" height="50%" />    
    
當 f = 0，則履約價K即為該遠期契約的初始價值，    

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Images/未命名3.jpg" width="30%" height="30%" />    
    
若該資產為股票，亦可將資產期望值前面的無風險利率，利用CAPM計算出的資產報酬率代入。    
#### 2. 選擇權避險    

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW4/Images/1-Common-Used-Greeks-in-Finance.png" width="30%" height="30%" />    
上述是一些有關於選擇權避險的方式，其中都和某項敏感度有關係。    
    
最常見的Delta Method便是選擇權對標的物價格敏感度，我們利用此項敏感度達到Delta neutral時，我們便對標的物價格造成的波動免疫。
