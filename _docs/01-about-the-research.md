---
title: "About the Research"
permalink: /docs/about-the-research/
excerpt: "Explanations about why learnfin package exists and resarch behind it."
modified: 2016-09-14T18:02:00-01:00
---

{% include base_path %}

Information below can get somewhat technical on the grounds of quantitative finance, option pricing and unsupervised learning. I'll try my best to avoid technicalities and jargon as best as possible to clearly state the problem and the objectives of this research.
{: .notice--warning}

## Problem Statement

**Summary:** It is a problem of prediction stability. We ask how much pricing error changes for similar option contract parameters if we change the data set. In addition, we ask is arbitrarily defined intervals the best way to capture pricing error information or if it could be done in a better way.
{: .notice--info}

In quantitative finance, it is important to correctly price assets and contracts on those assets (i.e. [options](#)). Therefore option pricing models are designed to estimate these prices. "Pricing error" occurs, when the price estimate of the model ($$\hat{P_i}$$) and the market price ($$P_i$$) for the contract $$i$$ differ.

Literature on option pricing usually groups pricing error values from many different contracts into intervals of moneyness (i.e. relative position of the spot price to the strike price; $$S_0/K$$) and maturity (i.e. time remaining to the expiration of the contract; $$T-t$$). For instance, see the pricing error table below.

<figure>
  <img src="{{ base_path }}/images/lehar-example.png" alt="Lehar Pricing Error Table">
</figure>

The pricing error table is from [Lehar et al. (2002)](http://www.sciencedirect.com/science/article/pii/S0378426601002254). There are three different option pricing models: Black Scholes (BS), Hull-White (HW) and GARCH. Pricing error type is relative pricing error (RPE); $$\dfrac{\hat{P_i}-P_i}{P_i}$$ ($$). The table tells us Black-Scholes (BS) model underprices option contracts that have moneyness between -0.02 and 0.02 and maturity between 0.4 and 0.6 by 10.71 (hence the negative sign).

Main question is **"If I repeat the same pricing experiment with another set of data, will the pricing error be same or similar for the same moneyness and maturity intervals?"**

TODO: Continue
