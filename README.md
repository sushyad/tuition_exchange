# tuition_exchange
Information about colleges and universities that participate in tuition exchange. The list of colleges and their participation levels was scraped from http://tuitionexchange.org. The costs and some admissions information associated with the various colleges was taken from the college scorecards https://collegescorecard.ed.gov/data/. For schools that don't participate in college scorecards, I wrote a script to scrape google searches for ACT scores associated with the college.

Note that the scorecard data is from 2015/2016. So, I scraped total cost of attendance for colleges I could find. For those I couldn't, I added about 7 per cent to the 2015/2016 total. 

The main dataset is in data/full_data.csv. There are errors and omissions in this data. I welcome any pull request that fixes any problem, no matter how small! The data contains 655 observations of the following variables

1. INSTNM - The name of the institution.
2. STABBR - the state abbreviation for where the institution is located.
2. cost_estimate - scraped or estimated total cost of attendance
3. low_act - the 25th percentile ACT score; either from scorecard or scraping.
4. mid_act - the median ACT score, from scraping.
5. high_act - the 75th percentile ACT score;ither from scorecard or scraping.
6. TUITIONFEE_OUT - out of state tuition from scorecard; some entered by hand.
7. ADM_RATE - admission rate from scorecard      
8. COSTT4_A - total cost of attendance from 2015/2016
9. UGDS - number of undergraduate students.
10. ACTCM25 - act composite 25th percentile
11. ACTCM75 - act composite 75th percentile
12. SATMT25 -sat math 25th percentile
13. SATMT75 - sat math 75th percentile
14. reward_type - tuition exchange reward type; either full, set rate or other
15. net_cost_2017_2018 - total cost adjusted for inflation minus either tuition (full tuition) or set rate (set rate or other).
16. net_cost_2018_2019_best_estimate - OK, this is my best estimate for what net cost will be if you get tuition exchange scholarship.
