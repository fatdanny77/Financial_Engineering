# Financial Engineering HW2
## [**Code**](https://github.com/fatdanny77/Financial_Engineering/blob/master/HW2/Financial%20Engineering%20HW2_ver2.ipynb)
#### 此次作業的Spot rate以及Forward Rate參考[網址1](https://www.trignosource.com/finance/spot%20rate.html#Calculator)以及[網址2](https://www.trignosource.com/finance/Forward%20rate.html#Calculator)，裡面的方式為直接計算一零息債券，因此本處亦同。   
     
## **Learning Process**
## 1. 債券定價修正
#### 前幾周已有講到債券的定價模式，然而若債券交易的時間點在兩次發放Coupon的間隔中，債券價格就需要將其納入考量。

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW2/figures/%E6%9C%AA%E5%91%BD%E5%90%8D.jpg" width="50%" height="50%" />

#### 其中𝓌為交易日期到下一次Coupon發放日的間隔。
## 2. Duration
#### 債券之存續期間為判定利率對於債券價格敏感度的指標。
#### (1.) Macaulay Duration

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW2/figures/%E6%9C%AA%E5%91%BD%E5%90%8D1.jpg" width="50%" height="50%" />

#### (2.) Modified Duration

<img src="https://github.com/fatdanny77/Financial_Engineering/blob/master/HW2/figures/%E6%9C%AA%E5%91%BD%E5%90%8D2.jpg" width="50%" height="50%" />

## 3. Spot Rate & Forward Rate
#### 由於我們先前計算的YTM為將債券持有至到期日的折現率，若我們希望計算債券持有的特定期間的報酬率，我們便在計算其Spot Rate及Forward Rate，其中Forward Rate是藉由兩段Spot Rate所計算出來的。至於計算方法，Spot Rate之計算只需將債券分割成無數個零息債券即可。
#### **P = F/(1 + r)^n**
where r is the spot rate
