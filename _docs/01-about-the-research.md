---
title: "About the Research"
permalink: /docs/about-the-research/
excerpt: "Explanations about why uslfin package exists and resarch behind it."
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

<!--
Minimal Mistakes has been developed to be 100% compatible with hosting a site on [GitHub Pages](https://pages.github.com/). To get up and running with a new GitHub repository quickly, follow these steps or jump ahead to the [full installation guide]({{ base_path }}/docs/installation/).

## Fork the Theme

Fork the [Minimal Mistakes theme](https://github.com/mmistakes/minimal-mistakes/fork), then rename the repo to **USERNAME.github.io** --- replacing **USERNAME** with your GitHub username.

<figure>
  <img src="{{ base_path }}/images/mm-theme-fork-repo.png" alt="fork Minimal Mistakes">
</figure>

**Note:** Your Jekyll site should be viewable immediately at <http://USERNAME.github.io>. If it's not, you can force a rebuild by **Customizing Your Site** (see below for more details).
{: .notice--warning}

If you're hosting several Jekyll based sites under the same GitHub username you will have to use Project Pages instead of User Pages. Essentially you rename the repo to something other than **USERNAME.github.io** and create a `gh-pages` branch off of `master`. For more details on how to set things up check [GitHub's documentation](https://help.github.com/articles/user-organization-and-project-pages/).

<figure>
  <img src="{{ base_path }}/images/mm-gh-pages.gif" alt="creating a new branch on GitHub">
</figure>

**ProTip:** Be sure to [delete](https://github.com/blog/1377-create-and-delete-branches) the `gh-pages` branch if you forked Minimal Mistakes. This branch contains the documentation and demo site for the theme and you probably don't want that showing up in your repo.
{: .notice--info}

## Customize Your Site

Open up `_config.yml` found in the root of the repo and edit anything under **Site Settings**. For a full explanation of every setting be sure to read the [**Configuration**]({{ base_path }}/docs/configuration/) section, but for now let's just change the site's title.

<figure>
  <img src="{{ base_path }}/images/mm-github-edit-config.gif" alt="editing _config.yml file">
  <figcaption>Edit text files without leaving GitHub.com</figcaption>
</figure>

Committing a change to `_config.yml` (or any file in your repository) will force GitHub Pages to rebuild your site with Jekyll. It should then be viewable a few seconds later at `https://USERNAME.github.io`.

---

Congratulations! You've successfully forked the theme and are up an running with GitHub Pages. Now you're ready to add content and customize the site further.
-->
