### Bonds

#### Characterstic of Bonds

* #### Par Value
Face value of the bond, returned to the bondholder at maturity

* #### Price
Represented as a percentage of face value of par.

* #### Coupon
Percentage of the pare value of bond that will be paid periodically in the form of interest
```
parValue=1000
couponRate=5%
AnnualReturn=1000*5% = 50
```

* #### Zero Coupon Bonds
    * Zero or low coupon rate
    * Don't pay interest
    * Issued at discount below par value

* #### Maturity
Length of time until bond issuer return the par value to the bondholder and terminates or redeems the bond

* #### Call Provision
Gives a corporation the option to redeem the bonds before the maturity date
If interest of bonds frop by 3% company can buy back the bond at re-issue at new interest rate in auction

* #### Yield
Rate of return the investor will earn on the bond after taking into account the price paid for the bond and the coupon on the bond. **Yield Curve** How much money is generated from the investment graph between yield and time
     * flat => its concern where short term and long term yield is close
    * inverted => short term have high return where long term have low return
    * normal => short term have low return where long term have high return

```
Yield = coupon/price
```

```
yieldToMaturity=(AnnualCouponInterestPayment+((FaceValue-Price)/YearsToMaturity))/(FaceValue+Price)/2
```

   


### Bond Rating
Reflects future risk potential of bonds

High Bond Ratings -- less probability to default
* AAA
* AA1
* AA2
* AA3
* A1
* A2
* A3
* BAA1
* BAA2
* BAA3

Lower Bond Ratings (Junk Bonds) -- higher probability to default
> High Yield
> Higher Interest rate compare to AAA Bond
* BA1
* BA2
* BA3
* B1
* B2
* B3
* CAA1
* CAA2
* CAA3
* CA

### Bond Valuation


```python

maturity=10       #year
interest=0.08     #percentage
par=1000
coupon=par*interest
par=1000
yields=0.08        #percentage

price=np.npv(rate=yields, nper=maturity, fv=coupon, pmt=0)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[1], line 8
          5 par=1000
          6 yields=0.08        #percentage
    ----> 8 price=np.npv(rate=yields, nper=maturity, fv=coupon, pmt=0)
    

    NameError: name 'np' is not defined


### Relation Between factor in Bonds

* price is inversly propotional to yield
* coupon and yeild
```
    if price < par
        yield is higher
    else if price > par 
        yield is lower
    else
        yield = coupon
```
* yield and maturity
```
    if maturity is higer 
        yield is high
    else
        yield is lower
```


### Types of Bonds

* #### Treasury Bonds
    * Safe securities
    * Control by government
    * issue short-term (T-Bills) and long-term (T-Bonds)
    * Pay face value at maturity
    * T-Bills sell at discounted price
    * T-Bonds that pay semiannual coupons in addition to thier face value at maturity
    * Lower interest rate

* #### Municipal (muni) Bonds
    Bonds issued by state and local government

    * Tax-Backed Bonds
        * Issued by states, country, distict, cities. town
        * Secured by tax Revenue
    * Revenue Bonds
        * Issued for special project
        * amount paid back by profit of project
    

