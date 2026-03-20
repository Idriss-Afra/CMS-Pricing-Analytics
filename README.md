# CMS Pricing Analytics

A quantitative finance repository focused on pricing **Constant Maturity Swap (CMS) derivatives** from interest-rate market inputs.

This project develops a replication-based framework for **CMS forwards**, **CMS caplets**, and **CMS spread options**, combining **normal-model swaption pricing**, **Hagan’s flat swap-curve approximation**, and **Carr-Madan static replication**.

---

## Repository Structure

```text
CMS-Pricing-Analytics/
├── CMS Derivatives Pricing Analytics.ipynb
```

---

## Project Overview

This notebook focuses on the pricing of **CMS-linked payoffs** in an interest-rate derivatives setting.

It starts from the valuation of a generic CMS payoff under the appropriate payment measure, then reformulates the problem under the **level (annuity) measure**, where the forward swap rate is a martingale. To make the pricing tractable, the project applies **Hagan’s flat swap-curve approximation**, which expresses the key measure-change term as a function of the terminal swap rate alone.

This reformulation allows the payoff to be priced through **Carr-Madan static replication** using **out-of-the-money European swaptions**. In this implementation, European swaptions are priced under the **normal (Bachelier) model**, and the framework is then applied to compute **CMS convexity-adjusted forwards**, **CMS caplet prices**, and **CMS spread option values**.

---

## Model Components

The implementation includes:

* **European swaption pricing** under the normal (Bachelier) model
* **Hagan’s flat swap-curve approximation**
* **Carr-Madan static replication**
* **CMS forward pricing**
* **CMS caplet pricing**
* **CMS spread option pricing**

---

## Example Output

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/6bf87e10-a92a-432c-b484-799018759783" />


---

## Best use case

Use this notebook when working with **interest-rate derivatives** and building a **CMS pricing framework** for convexity-adjusted forwards, vanilla CMS options, and CMS spread option valuation.

---

## How to Use

Clone the repository:

```bash
git clone https://github.com/Idriss-Afra/CMS-Pricing-Analytics.git
cd CMS-Pricing-Analytics
jupyter notebook
```

Then open:

* `CMS Derivatives Pricing Analytics.ipynb`

---

## Author

**Idriss Afra**
