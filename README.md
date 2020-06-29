# LendingClub Loan Status Classifier

LendingClub is a facilitator of peer-to-peer loans. The company makes money by charging borrowers an origination fee, and investors a service fee.

This project aims to create a classifier that predicts the status of loans made through LendingClub. Loan status in this case is divided into two categories: **troubled** and **non-troubled**, where troubled is defined as a loan meeting at least one of the following criteria:
1. Defaulted
2. Delayed past the initial 15 day grace period
3. Completely charged off (LendingClub does not expect payment). Loans are typically charged off after 120 days of failed payments.

**Loan Quick Facts:**
* Loan principal amounts are between 1,000 and 40,000 USD
* The term of the loan is either 3 or 5 years

Data
---
Data is pulled from https://www.lendingclub.com/statistics/additional-statistics? (login required).
