#### Investment

* Stock Market
* Bonds
* Mutual Funds
* Exhange Traded Fund
* Commodity Market
* Fixed Income
* Fixed Depoiste
* Recurring Deposite

## Capital Market = Stocks + Bonds

* #### Bond Market
Its similar way of giving loan to a company for particular time period 

* #### Treasury Bills (T-Bills)
Short term bonds issued by the Treasury that mature in less than a year

* #### Equity
Its a system that enables companies to sell partial ownership in themselves to people in exchange for cash

* #### Exhange Traded Fund (ETF)
Its an basket of multiple stock where the invested amount is distributed in all stock present in ETF as per thier weightage

#### Diversification

Instead of investing all money at one place, invest in multiple places, to achieve diversification it can be achieved from few ways:
* RealState, Stock, Index Fund, FixedDeposite
* Invest in Stock distribute the invested amount in multiple sector
* Invest in Stock as well as in internation Stock (Invest in Internation Sotck can be done by investing ADR or opening account in the country firm)

#### Shrinking Stock Market

Size of the market is same, no of share get reduce to trade
It happen in few ways
* Large companines buy smaller one
* Some of them going to public
* No of share is decreasing over the period of time (Ex: Buyback)

##### Issue:
* Difficult to find good stock

#### Valuation:
Valuation is the analytical process of determining the current (or projected) worth of an asset or a company.

Valuation = ExpectedDivedend/(RequriredRateOfReturn-GrowthRate)


```python
stock_name='Microsoft'

last_year_dividend=1.84

#In Billion
last_year_total_revenues_2017 = 96.57
current_year_total_revenues_2018 = 110.36


growth_rate = (current_year_total_revenues_2018-last_year_total_revenues_2017)/last_year_total_revenues_2017*100
expected_divdend = (growth_rate/100+1)*last_year_dividend

#18% assumption for current year
required_rate_of_return = 18

valuation=expected_divdend/((required_rate_of_return-growth_rate)/100)

print(valuation)
```

    56.522407170294606
    

#### Earning Per Share (EPS)
Earnings per share (EPS) is calculated as a company's profit divided by the outstanding shares of its common stock. The resulting number serves as an indicator of a company's profitability. It is common for a company to report EPS that is adjusted for extraordinary items and potential share dilution.

```
EPS=(netIncome-annualDividend)/shares
```

### Types of Ways to get Share

#### Equity Share
* Common Stocks
> It allow individual to enjoy the profits of the issuing company in form of dividends paid to the shareholders.
> Ownership
> voiting rights
> dividends

* Preference Share
> A preference share enables a shareholder with a right to obtain regular dividends from a company
> Preference share over the common shares during payment o dividends or during liquidation of the company


#### Primary Market
* Deal with issuance of new securities
* Shares can be bought directly from the issuing company

* #### Intial Public Offereing (IPO)
> * If company sells its share to individuals investors for the first time it is referred as IPO

* #### ESOP
> Employee can acquire stock of the company as a part of the compensation or rewards program

#### Secondary Market
Shares are have already bought and sold, it operate by the exchanges to insure safety and trade.

#### Factors Affecting Price of Stocks
* Market News +ve or -ve
* Price Momentum in international market
* Price change in similar stocks
* Earnings of Company 


## Corporate Action
Any event that brings material change to a company and affect its stakefolder

* #### Stock Split
Increase no of share in market without impacting total outstanding shares, Price is adjusted such as MarketCap before and after Stock Split is same.


```python
#Stock Split 2:1
no_of_share=100
price=50
before_market_cap=no_of_share*price

split_for_share=1
split_given_share=2

after_no_of_share=no_of_share/split_for_share*split_given_share
after_price=price/split_given_share
after_market_cap=after_no_of_share*after_price

print("before_market_cap = ", before_market_cap)
print("after_market_cap = ", after_market_cap)
```

    before_market_cap =  5000
    after_market_cap =  5000.0
    

* #### Reverse Stock Split (Consolidation)
No of total outstanding value get decrease where price per share get increase without impacting the market cap


```python
#Reverse Stock Split 2:1

no_of_share=100
price=50
before_market_cap=no_of_share*price

split_for_share=1
split_given_share=2

after_no_of_share=no_of_share/split_given_share*split_for_share
after_price=price*split_given_share
after_market_cap=after_no_of_share*after_price

print("before_market_cap = ", before_market_cap)
print("after_market_cap = ", after_market_cap)
```

    before_market_cap =  5000
    after_market_cap =  5000.0
    

* #### BuyBack (Tender Offer)
Company offers to buy back its shares at a premium. It possible it happen to increase value of share by decreasing the supply or eliminate threats by operators.

* #### Bonus Share
Issue fresh shares to distibute profits to shareholders called bonus issue effect the price. To encourage retails participation by increasing their equity base.
No of share increase where price will not impact, give advantage for tax exemption


```python
# Bonus of 2:1 (2 share for every 1 share)
no_of_share=100
price=50
before_market_cap=no_of_share*price

split_for_share=1
split_given_share=2

after_no_of_share=no_of_share+(no_of_share/split_for_share*split_given_share)
after_price=price
after_market_cap=after_no_of_share*after_price

print("before_market_cap = ", before_market_cap)
print("after_market_cap = ", after_market_cap)
```

    before_market_cap =  5000
    after_market_cap =  15000.0
    

* #### Dividend
It is distribution of profits by the issuer to its shareholders. Percentage of dividend is define from the face value of the share
Price of share is fall down once dividend is paid. Price is depend on multiple factor its possible it will not refelect in numbers.

```
Dividend(%) = DividendAmount/FaceValue*100
```

``` 
Price = priceBeforeDividend - DividendAmount
```


* #### Rights Issue/Open Offer
Company offeres new shares to existing shareholders. Offers of shares or convertible securities made to existing shareholder on a record date, It offer in particular ratio with reference to share held on record date

* #### Warrants
Right to buy shares in a company in the future on agreed terms.

* #### TakeOver
A predator makes a bid for your share

* #### Conversion (debt to equity)
Debt holders have the option to convert it shares

* #### Repayment/Redemtion
Company may pay back capital to share and/or stake holders

### Types of Trader

* #### Scalper
100 of trade in day, earn profit by effective use of spread (difference in bid and ask trade)

* #### Momentum Trader
Identify high vloume stocks, Leverage by momentum gain/loss

* #### Techincal Trader
Analyze charts and graph, invest based on pattern

* #### Fundamental Trader
Invest based on fundamental analysis by study balance sheet, income, Splits, acquisition based on undervalue or over valued share

* #### Swing Trader
Share for days earn profits by changing in price effect by sentiment, corporate action etc

* #### Day Trader
Take position and close the position on same day

### Types of Order

* #### Market Order
Stock sold and bought at market price

* #### Limit Order
Trader mention limit of buy/sell the stocks, It also use to manage the risk 
sell >= sellLimit
buy <= buyLimit

* #### Day Order
Buy and sell stock in same day, If order are not execute it will not carry over to next day

* #### Good Till Cancelled Order (GTC)
Order buy or sell at specific limit order, Order is unexecuted till the limit price come in range as per the limit specified


* #### Good Till Date (GTD)
Order remain unexecuted till the date specified by the trader

* #### All or None Order (AON)
It either execute all or non order. It an open order until full quantity satisfied

* #### Immediate or Cancel Order (IOC)
It either execute (complete or partially) or get cancelled upon being placed

* #### Fill or Kill (FOK)
Buy or sell a stock that must be executed immediately else it get cancelled.

* #### Drip Feed
slowly advancing funds or capital in stages rather than injecting a large lump sum right off the bat.

## Trading Strategy

* #### Buy and Hold
Invested over long period of time for long-term, Its a safest option based on multiple resarch. It also gives an advantage of time and tax exemption

* #### Market Timing
Trader follow the market based on charts to decide when to buy and sell. Sell stokcs when market are high and buy when it low

* #### Value Stocks
Invest in Underpriced and penny stock, calculate expected price and determine under or over valued
> * Modestly priced
> * Mature Firms
> * More Stable
> * Indutries that aren't rapidly growing
> * Exapmle: Railroad, Utility, Industrial equipments makers, Energy providers

* #### Growth Stocks
Invest in growth potential. Perform fundamental anlaysis to predict who well stock do in future based on below factors
* Fast Growing
* Lower profit
* Relatively expensive
* Price drop to some specific condition
* Example: IT, etc


* #### Growth at Resaonable Price (GARP)
It follow both Growth and Value, Undervalued with growth potential

* #### Income
Trader focus on Highly Dividend instead of capital gain. 

* #### Contrarian
Operating against the current market moment.

* #### Canslim
Invest after Fundamental and Technical Analysis. Good for those can hold for long term
> * C = Current Quaterly Earing per year (compare last 3 quater)
> * A = Growth in annual earning (27% annual and 15%ROI)
> * N = new product, services, leadership, pricing condition introduce
> * S = Supply and demand
> * L = Knowing Leader and laggers based on sector
> * I = Instidutional support (more support will good)
> * M = Market direction (bullish and bearish)


* #### Hedging
It best strategy it insure protection of capital. Holding risk stocks by holding certain stokcs. Hedger takes short position to offset the long positions

* #### Dogs of the Dow
10 best performing stocks in the year with Lowest P/E raios, Highest dividend yields and potential for high growth are slected

* #### Pigs of the Dow
10 worst performing socks in the year , Stocks are sure to rebound

* #### Buying on Margin
It riskiest strategy trader borrowing money from broker.

* #### Dollar Cost Averaging
Invest Fixed amount in share, If price down investor buy more share, average price per share goes down. If price raise new share give good benefit.

* #### Value Averaging
Trader decide to invest based on market mood if market is bull invest more, if its bear invest less

* #### Market Neutral 
Trader take long-position on undervalued and short-position on overvalued. It help to diversified and commonly use in hedge.

* #### Directional
Trader make benifit when market go up and when market go down

* #### Event Driven
Trader make profit by the event happen in stocks (dividend, corporate action)

## Derivaties 

### (Option Trading)
Contract between two partied to exchange a stock at a "strike" price by a predetmined date. 

* #### Call
Buyer of the call has right but no obligation to buy the stock at strike price by the future date, while the seller of the call, has the obligation to sell the stock to the buyer at the strike price if the buyer exercises the option.

* #### Put
Buyer of the put has right but no obligation to sell the stock at strike price by the future date, while the seller of the put, has the obligation to buy the stock to the buyer at the strike price if the buyer exercises the option.

### Trade Life Cycle

Trading -> Clearing -> Settlement

