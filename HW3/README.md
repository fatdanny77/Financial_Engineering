# Financial Engineering HW3
## [I. Code](https://github.com/fatdanny77/Financial_Engineering/blob/master/HW3/Codes/Financial_Engineering_HW3_ver2.ipynb)

## [II. Flow Chart](https://github.com/fatdanny77/Financial_Engineering/blob/master/HW3/FlowCharts/Flow_Chart.jpg)
## III. Learning Process

### 1. 買權 (Call)
能夠在到期時以履約價格買進標的物的權力，通常在預期未來標的物價格上漲時購買。

### 2. 賣權 (Put)
能夠在到期時以履約價格賣出標的物的權力，通常在預期未來標的物價格下跌時購買。

### 3. 債券評價
#### (1.) Put-Call Pairty
> ### **C + Ke^rt = P + S**    
where
* C = call premium
* Ke^rt = present value of strike price
* P = put premium
* S = the current price of the underline    

這裡的Ke^rt可以想像賣空K單位債券折現回來，買了C。

#### (2.) Black-Scholes Model
假設時間為連續，股價呈常態分配。   

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW3/Images/%E6%9C%AA%E5%91%BD%E5%90%8D4.jpg" width="50%" height="50%" />

#### (3.) Binomial Option Pricing Model (BOPM)
假設時間為離散，由最後一期之選擇權價值反推現值。   

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW3/Images/%E6%9C%AA%E5%91%BD%E5%90%8D2.jpg" width="50%" height="50%" />
若為賣權，則為 max(K-S,0)。特別注意，這裡的q不是投資人主觀的上漲機率，而是由風險中立算出的機率。投資人的主觀機率已反映在股價上。
