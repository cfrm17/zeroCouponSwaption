# Zero Coupon Swaption Valuation

A zero-coupon swaption is an option on a zero coupon swap in which no coupon is paid before the swap maturity. The final floating side payment is compounded from the pre-determined fixed rate. There are many different types of swaps.

The study shows that pricing an interest rate zero coupon swaption is equivalent to pricing a corresponding variable notional and fixed rate swaptions. An interest rate variable notional and fixed rate (VNFR) swap is a fixed rate versus floating rate swap when notional principals and fixed rates/floating spread may not uniformly be specified through swap periods. A variable notional and fixed rate swaption is an option on a VNFR swap.

A VNFR swap is different from a traditional vanilla swap that for the former, the concept of vanilla swap rate may not be directly applied to a VNFR swap. The traditional approach may still be applicable after the modified concept of “swap rate”, which may be called a VNFR swap rate, is introduced to the VNFR swap. 

However, unlike volatilities of the vanilla swap rates, volatilities of the VNFR swap rates
are not directly market observable since European VNFR swaptions are not considered as liquid products in the swaption market. Therefore, how to estimate those volatilities through vanilla swap rate volatilities becomes crucial. A practical approach to estimating VNFR swap rate volatilities has been proposed

Under some conditions, which will be provided later, zero coupon swaps can be considered as examples of variable notional and variable coupon/spread (VNCS) swaps. The following analysis will prove the equivalences. Let

t — generic valuation time point;
DCB — day-count basis;
dcf — day-count fraction of a period with a given DCB;
Dst — discount factor at the time of s to the time of t, s _ t;
C(·) — cash flow function with respect to time;
PV(t,C) — present value of a cash flow C at a time of t;
β — index of pay-fixed (+1) and receive-fixed (−1).

Let us consider an interest rate swap which is composed of the following fixed-leg and floating-leg. Let m > 0 be a given integer, tx0 < tx1 < · · · < txm be roll dates of the fixed-leg, in which, tx0 is called a (fixed-leg) start (or effective) date and tx m a (fixed-leg) maturity. The ith sub-period of the leg is defined as [tx i−1, txi] and _x i = dcf([tx i−1, txi ]), i = 1, · · · , m.  corresponding to each sub-period [tx i−1, txi], ci is the fixed coupon rate with simple compounding. Define

 

By using the induction, we have

 

A Zero-Coupon (ZC) fixed leg can be defined as a forward contract with the following cash flow,
denoted by CZC X(·), which is given by

 

where δ(·) is the Kronecker function. Similarly, a ZC-floating leg can be defined as a forward contract with the following cash flow, denoted by CZC F(·), which is given by

 

Then, corresponding to the above defined ZC-fixed leg and ZC-floating leg, the pay-fixed ZC-swap can be defined as the portfolio of short the ZC-fixed leg and long the ZC-floating leg whose cash flow, denoted by CZCS RTP(·), is given by

 

The receive-fixed ZC-swap can be defined as the forward contract with following cash flow

 

In order to implement our valuation procedure, we need to model the dynamics of the term structure. One way to achieve the goal is to model the short rate. 

To price a Bermudan zero coupon swaption, A binomial tree approach is used to price the Bermudan option on zero coupon swap. Therefore, a constant volatility of an underlying rate must be applied. This constraint is inadequate to handle a volatility term structure.

The calculation of the constant volatility depends on a correlation matrix which may be subjective and twisted. In some severe cases, the correlation matrix may not maintain its semi-positive definite property.

An alternative approach is proposed to price Bermudan zero coupon swaptions based on Bermudan variable notional swaption model. It has been proved that a zero coupon swaption, under some normal conditions, is a special case of a variable notional swaption. The transformation of a Bermudan zero coupon swaption into a Bermudan variable notional swaption is straightforward.

Reference:

https://finpricing.com/knowledge.html

