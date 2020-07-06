# LendingClub Loan Status Classifier

Overview
---
LendingClub is a facilitator of peer-to-peer loans, connecting borrowers with investors. Borrowers begin by first submitting loan applications, which are then evaluated to determine if they are suitable to be listed on LendingClub's platform. If a loan is found to be suitable, LendingClub's model assigns it an interest rate based on the credit risk of the borrower, and investors can then decide whether to fund the loan by committing capital. The company makes money by charging fees to both sides (an origination fee to borrowers, and a service fee to investors).

This project aims to create a model that predicts whether loans made through LendingClub will be fully paid off or not. The motivation for such a model is apparent: investors aim to maximize returns by minimizing losses of principal and interest.

Predictions made by the model will be tested by comparing the returns on loans deemed "safe" by the model, to a broader population of loans. If an investor can use these predictions to identify loans that default less on average than a broader sample, some value may be added to the investment selection process.

Data
---
**Source:** https://www.lendingclub.com/statistics/additional-statistics? (login required).
**Time Frame:** Loans issued between 1/2010 and 12/2016

**Loan Details:**
* Loan principal amounts are between 1,000 and 40,000 USD
* Loans are paid back over a period of either three or five years, though prepayments can be made

Note: Employer Title replaces the Employer Name field for all loans listed after 9/23/2013

Methodology
---
To exclude loans whose ultimate payment status has not yet been determined (i.e. loans still outstanding), loans were only included if they were **Charged off**, **Defaulted**, or **Fully Paid**.

Loans are determined to be in default when payments have not been made for an extended period of time. Generally, if the borrower continues to fail to make payments for 120 days, further payments are not expected and the loan status shifts to charged off.

Results
---
