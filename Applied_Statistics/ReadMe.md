
<b>Think Stats</b>
* Download the book here: http://greenteapress.com/thinkstats/

********************************************************************************

<b>Data Source</b>

* 2002 Preganent Data: ftp://ftp.cdc.gov/pub/Health_Statistics/NCHS/Datasets/NSFG/2002FemPreg.dat
  * Data Dictionary: ftp://ftp.cdc.gov/pub/Health_Statistics/NCHS/Datasets/NSFG/stata/2002FemPreg.dct
* 2002 Respondent Data: /Health_Statistics/NCHS/Datasets/NSFG/2002FemResp.dat
* About NSFG Survey: https://www.icpsr.umich.edu/nsfg6/
* My code - Read Raw Data: https://github.com/hanhanwu/Hanhan_Data_Science_Practice/blob/master/Applied_Statistics/read_nsfg_data.py
  * preg output: https://github.com/hanhanwu/Hanhan_Data_Science_Practice/blob/master/Applied_Statistics/2002FemPregOut.csv
    * <b>birthorder</b> is empty when it's not live birth...
    * <b>finalwgt</b> is the statistical weight associated with the respondent. It is a floating-point value that indicates the number of people in the U.S. population this respondent represents. Members of oversampled groups have lower weights.
  * resp output: https://github.com/hanhanwu/Hanhan_Data_Science_Practice/blob/master/Applied_Statistics/2002FemRespOut.csv


* Other Data Sources
  * WalframAlpha: http://www.wolframalpha.com/
  

********************************************************************************

<b>Practice Code</b>

* [My Code - Chapter 1][1]

********************************************************************************

<b>Learning Notes</b>

* Mean describes the central tendency, while Variance describes the spread
* `Variance = sum(sqrt(Xi-mean))/n, i = 1,...,n`
  * `Xi-mean` is the deviation from the mean, so variance is mean squared deviation
  * People use standard deviation because it can more meaningful than variance. Variance us using squared unit (such as squared pund) but standard deviation is using unit (such as pound)
* Relative Risk - a ratio of 2 probabilities
  * For example, first born babies have 20% probability to be born late, other babies have 15%. Relative Risk will be 1.3 here. So first born babies have 30% more likely to be late
* Conditional Probability
  * We all know it means the probability under a certain condition, but I didn't think too much about its practical use
    * For example, it's 38th week now, and you want to know the probability of a born to be born next week (39th week). To calculate this probability, you can just check 39th week to 45th week numbers, and calculate the probability among them, instead of calculating the probability among 1st week to 45th week. I know, it sounds so simple....

[1]:https://github.com/hanhanwu/Hanhan_Data_Science_Practice/blob/master/Applied_Statistics/thinkstats_chapter1.ipynb