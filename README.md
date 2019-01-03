# loan-calc-snowball
Simple console program for calculating snowball payments for two loans with PMI and fixed interest rates.

# LoanCalc

Use spacebar to advance to the next year until all payments are complete.

# Default values in `%APPDATA%/pmh_software/LoanCalc.ini`

The ini file is located at `%APPDATA%/pmh_software/LoanCalc.ini`

These values will be generated on the first run of the exe, if the file isn't present.

	[General]
	extra_principle_per_month=0
	percent_paid_toward_first_loan=0.5
	verbose_output=true

	[house]
	loan_amount=100000
	pmi_per_month=100
	annual_interest_rate=0.03
	number_of_years=30
	loan_to_value=0.2

	[condo]
	loan_amount=100000
	pmi_per_month=100
	annual_interest_rate=0.03
	number_of_years=30
	loan_to_value=0.2

# Sample Output (abridged)

Years 2-27 are excluded. See output.txt for the full output.

	house
	  Length:     30 yr
	  Loan Amnt:  $100000
	  PMI/mo:     $100.00 for first 20.0%
	  Annual Int: 3.0 %
	condo
	  Length:     30 yr
	  Loan Amnt:  $100000
	  PMI/mo:     $100.00 for first 20.0%
	  Annual Int: 3.0 %
	house    1       99828   250.00  100.00  1.00    521.60 521.60  0.00
	house    2       99656   249.57  100.00  1.00    1043.20        521.60  0.00
	house    3       99484   249.14  100.00  0.99    1564.80        521.60  0.00
	house    4       99311   248.71  100.00  0.99    2086.40        521.60  0.00
	house    5       99138   248.28  100.00  0.99    2608.00        521.60  0.00
	house    6       98964   247.84  100.00  0.99    3129.60        521.60  0.00
	house    7       98790   247.41  100.00  0.99    3651.20        521.60  0.00
	house    8       98615   246.97  100.00  0.99    4172.80        521.60  0.00
	house    9       98440   246.54  100.00  0.98    4694.40        521.60  0.00
	house    10      98265   246.10  100.00  0.98    5216.00        521.60  0.00
	house    11      98089   245.66  100.00  0.98    5737.60        521.60  0.00
	house    12      97912   245.22  100.00  0.98    6259.20        521.60  0.00

	condo    1       99828   250.00  100.00  1.00    521.60 521.60  0.00
	condo    2       99656   249.57  100.00  1.00    1043.20        521.60  0.00
	condo    3       99484   249.14  100.00  0.99    1564.80        521.60  0.00
	condo    4       99311   248.71  100.00  0.99    2086.40        521.60  0.00
	condo    5       99138   248.28  100.00  0.99    2608.00        521.60  0.00
	condo    6       98964   247.84  100.00  0.99    3129.60        521.60  0.00
	condo    7       98790   247.41  100.00  0.99    3651.20        521.60  0.00
	condo    8       98615   246.97  100.00  0.99    4172.80        521.60  0.00
	condo    9       98440   246.54  100.00  0.98    4694.40        521.60  0.00
	condo    10      98265   246.10  100.00  0.98    5216.00        521.60  0.00
	condo    11      98089   245.66  100.00  0.98    5737.60        521.60  0.00
	condo    12      97912   245.22  100.00  0.98    6259.20        521.60  0.00

	Year SubTotal Paid: 12518.40

	------------------------------
			   Year 1
	------------------------------
	Name  Month  Balance  Interest  PMI  LtV  TotalPaid  MonthPmnt  ExtraPrinciple
	house    13      97735   244.78  100.00  0.98    6780.80        521.60  0.00
	house    14      97558   244.34  100.00  0.98    7302.40        521.60  0.00
	house    15      97380   243.90  100.00  0.97    7824.00        521.60  0.00
	house    16      97202   243.45  100.00  0.97    8345.60        521.60  0.00
	house    17      97024   243.01  100.00  0.97    8867.20        521.60  0.00
	house    18      96845   242.56  100.00  0.97    9388.80        521.60  0.00
	house    19      96665   242.11  100.00  0.97    9910.40        521.60  0.00
	house    20      96485   241.66  100.00  0.96    10432.00       521.60  0.00
	house    21      96305   241.21  100.00  0.96    10953.60       521.60  0.00
	house    22      96124   240.76  100.00  0.96    11475.20       521.60  0.00
	house    23      95943   240.31  100.00  0.96    11996.80       521.60  0.00
	house    24      95761   239.86  100.00  0.96    12518.40       521.60  0.00

	condo    13      97735   244.78  100.00  0.98    6780.80        521.60  0.00
	condo    14      97558   244.34  100.00  0.98    7302.40        521.60  0.00
	condo    15      97380   243.90  100.00  0.97    7824.00        521.60  0.00
	condo    16      97202   243.45  100.00  0.97    8345.60        521.60  0.00
	condo    17      97024   243.01  100.00  0.97    8867.20        521.60  0.00
	condo    18      96845   242.56  100.00  0.97    9388.80        521.60  0.00
	condo    19      96665   242.11  100.00  0.97    9910.40        521.60  0.00
	condo    20      96485   241.66  100.00  0.96    10432.00       521.60  0.00
	condo    21      96305   241.21  100.00  0.96    10953.60       521.60  0.00
	condo    22      96124   240.76  100.00  0.96    11475.20       521.60  0.00
	condo    23      95943   240.31  100.00  0.96    11996.80       521.60  0.00
	condo    24      95761   239.86  100.00  0.96    12518.40       521.60  0.00

	Year SubTotal Paid: 12518.40
	
	... ... ... ...
	
	------------------------------
           Year 28
	------------------------------
	Name  Month  Balance  Interest  PMI  LtV  TotalPaid  MonthPmnt  ExtraPrinciple
	house    337     6625    17.82   0.00    0.07    175779.20      521.60  100.00
	house    338     6119    16.56   0.00    0.06    176300.80      521.60  100.00
	house    339     5613    15.30   0.00    0.06    176822.40      521.60  100.00
	house    340     5106    14.03   0.00    0.05    177344.00      521.60  100.00
	house    341     4597    12.76   0.00    0.05    177865.60      521.60  100.00
	house    342     4087    11.49   0.00    0.04    178387.20      521.60  100.00
	house    343     3575    10.22   0.00    0.04    178908.80      521.60  100.00
	house    344     3063    8.94    0.00    0.03    179430.40      521.60  100.00
	house    345     2549    7.66    0.00    0.03    179952.00      521.60  100.00
	house    346     2033    6.37    0.00    0.02    180473.60      521.60  100.00
	house    347     1517    5.08    0.00    0.02    180995.20      521.60  100.00
	house    348     999     3.79    0.00    0.01    181516.80      521.60  100.00

	condo    337     6625    17.82   0.00    0.07    175779.20      521.60  100.00
	condo    338     6119    16.56   0.00    0.06    176300.80      521.60  100.00
	condo    339     5613    15.30   0.00    0.06    176822.40      521.60  100.00
	condo    340     5106    14.03   0.00    0.05    177344.00      521.60  100.00
	condo    341     4597    12.76   0.00    0.05    177865.60      521.60  100.00
	condo    342     4087    11.49   0.00    0.04    178387.20      521.60  100.00
	condo    343     3575    10.22   0.00    0.04    178908.80      521.60  100.00
	condo    344     3063    8.94    0.00    0.03    179430.40      521.60  100.00
	condo    345     2549    7.66    0.00    0.03    179952.00      521.60  100.00
	condo    346     2033    6.37    0.00    0.02    180473.60      521.60  100.00
	condo    347     1517    5.08    0.00    0.02    180995.20      521.60  100.00
	condo    348     999     3.79    0.00    0.01    181516.80      521.60  100.00

	Year SubTotal Paid: 12518.40
	------------------------------
			   Year 29
	------------------------------
	Name  Month  Balance  Interest  PMI  LtV  TotalPaid  MonthPmnt  ExtraPrinciple
	house    349     480     2.50    0.00    0.00    182038.40      521.60  100.00
	house    350     0       1.20    0.00    0.00    182519.60      481.20  59.60
	Paid off Both Loans!!!

	condo    349     480     2.50    0.00    0.00    182038.40      521.60  100.00
	condo    350     0       1.20    0.00    0.00    182519.60      481.20  59.60
	Paid off Both Loans!!!

	Year SubTotal Paid: 2005.60
	ExPrinciple/mo, %ForFirstLoan,Name       TotalInterestPaid       TotalPmiPaid    TotalPaid       MonthsToPayOff
	0       0.5     house   51519.60        31000   182519.60       351
	0       0.5     condo   51519.60        31000   182519.60       351
	0       0.5     Sum     103039.20       62000   365039.20       351
	
# Pseudo Code

	Inputs:

	Total available extra principal per month
	Percent paid toward M1

	Mortgage 1
	Beginning Balance
	Interest rate
	Length of mortgage (in years)
	Start date
	PMI_initial
	Additional monthly principal payment

	Mortgage 2
	Beginning Balance
	Interest rate
	Length of mortgage (in years)
	Start date
	PMI_initial
	Additional monthly principal payment


	Some formulas
	AMPP1 = TAEPPM*PPTM1
	AMPP2 = TAEPPM-AMPP1

	If Current_loan1_balance/M1BB <= .8 , PMI_current = 0
	If Current_loan2_balance/M2BB <= .8 , PMI_current = 0

	If PMI_current = 0 , TAEPPM = TAEPPM + PMI_initial

	If current_loan1_balance <= 0, TAEPPM = TAEPPM + loan1_principal_and_interest
	If current_loan2_balance <= 0, TAEPPM = TAEPPM + loan2_principal_and_interest


	Things for which i do not have a formula, but there is probably a slick function already in existence or you could read in from a spreadsheet
	scheduled_payment1 (ie principal_and_interest)
	loan_balance1 at time step t
	principal_payment1 at time step t
	interest_payment1 at time step t

	scheduled_payment2 (ie principal_and_interest)
	loan_balance2 at time step t
	principal_payment2 at time step t
	interest_payment2 at time step t

	(note that although principal and interest change with each time step, principal + interest remains constant)

	Other things that will be needed but are really easy to get
	total_interest_paid_on_loan1 = sum(interest payment from t = 0 through t = (length of mortgage *12)
	total_principal_paid_on_loan1 = sum(principal payment from t = 0 through t = (length of mortgage *12)
	total_cost_of_mortgage1_without_extra_payments = scheduled payment *(length of mortgage *12)
	money_saved1 = total cost of mortgage without extra payments - (total interest paid + total principal paid)

	total_interest_paid_on_loan2 = sum(interest payment from t = 0 through t = (length of mortgage *12)
	total_principal_paid_on_loan2 = sum(principal payment from t = 0 through t = (length of mortgage *12)
	total_cost_of_mortgage2_without_extra_payments = scheduled payment *(length of mortgage *12)
	money_saved2 = total cost of mortgage without extra payments - (total interest paid + total principal paid)

	Total_money_saved = money_saved1 + money_saved2

## GOAL

Try every value for PPTM1 from 0 to 1 (step size = .01). Solution is when M1 and M2 balance is zero and total money saved is maximized.
bonus points...find the value for PPTM1 such that total time to bring M1 and M2 balance to zero is shortest.
