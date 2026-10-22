# The Jevons Dividend: sources

*By Srujan Valisetti.* The printed book gives a short reference for each source it draws on. This page gives the full note behind each one: the source, where in it the figure or quotation is found, any calculation of our own, any caveat, and a web address where there is one. Notes are numbered as in the printed book, chapter by chapter.

## Chapter 1: The Coal Question

**Note 1.**

> Coal burned in Scotland's iron industry rose tenfold.

W. S. Jevons, *The Coal Question* (1865), ch. VII: "the reduction of the consumption of coal, per ton of iron, to less than one-third of its former amount, has been followed, in Scotland, by a ten-fold total consumption". Jevons credits the growth "in some part" to "the use of the hot blast in smelting". https://www.econlib.org/library/YPDBooks/Jevons/jvnCQ.html?chapter_num=9

**Note 2.**

> "It is wholly a confusion of ideas," he wrote, "to suppose that the economical use of fuel is equivalent to a diminished consumption. The very contrary is the truth."

Jevons, *The Coal Question*, ch. VII.

**Note 3.**

> Jevons pointed to "the indirect effect of cheap iron in accelerating other coal-consuming branches of industry."

Jevons, *The Coal Question*, ch. VII.

**Note 4.**

> "As a rule," he wrote, "new modes of economy will lead to an increase of consumption according to a principle recognised in many parallel instances."

Jevons, *The Coal Question*, ch. VII.

**Note 5.**

> By October 2024, a model with the same score on a standard test of general knowledge cost 7 cents for the same million tokens.

Stanford HAI, *AI Index Report 2025*: from $20.00 per million tokens (November 2022) to $0.07 (October 2024, Gemini-1.5-Flash-8B) for a model scoring 64.8 on the MMLU benchmark. https://hai-production.s3.amazonaws.com/files/hai_ai_index_report_2025.pdf

**Note 6.**

> The price of a model that could pass a test of graduate-level science questions more than half the time went from $15 per million tokens in May 2024 to 12 cents in December of the same year.

*AI Index Report 2025*: the GPQA benchmark above 50%, from $15 per million tokens (May 2024) to $0.12 (December 2024, Phi 4).

**Note 7.**

> Researchers who track these prices estimate that, depending on the task, the cost of running AI models has been falling somewhere between 9 and 900 times a year.

Epoch AI estimate, quoted in the *AI Index Report 2025*.

**Note 8.**

> On 29 October, Sundar Pichai told investors the figure had passed 1.3 quadrillion, "more than 20x growth in a year." He added that customers using Google's models directly were sending seven billion tokens a minute, and that the Gemini app had more than 650 million users a month.

Alphabet Q3 2025 earnings call, 29 October 2025. https://s206.q4cdn.com/479360582/files/doc_events/2025/Oct/29/2025_Q3_Earnings_Transcript.pdf

**Note 9.**

> Critics point out that newer models which "think" before answering produce many tokens nobody reads, so raw token counts flatter real use.

A critic's view: The Decoder, "Google boasts 1.3 quadrillion tokens each month, but the figure is mostly window dressing". https://the-decoder.com/google-boasts-1-3-quadrillion-tokens-each-month-but-the-figure-is-mostly-window-dressing/

**Note 10.**

> Their own judgement was that in most cases it wouldn't go above about 60%, and most measured cases were well below that.

Gillingham, Rapson and Wagner, "The Rebound Effect and Energy Efficiency Policy", *Review of Environmental Economics and Policy* 10(1), 2016. Figures from the working-paper version (2015). https://files.gwagner.com/production/uploads/Rebound_Effect_GRW.pdf

**Note 11.**

> So history alone can't tell you which side your own market is on.

Our calculation, pre-registered test T3-A (analysis/PREREGISTRATION.md), code in `analysis/part3/t2_t3/`, results in
`analysis/results_part3_t2_t3.json`, red-team checks in `analysis/part3/redteam/rt_t3.py` and `rt_t3.json` (summary
in `analysis/part3/redteam/REDTEAM.md`, T3-A). Data: BEA, National Income and Product Accounts, Table 2.4.5
"Personal Consumption Expenditures by Type of Product" and Table 2.4.4 "Price Indexes for Personal Consumption
Expenditures by Type of Product", annual, flat files at https://apps.bea.gov/national/Release/TXT/ (NipaDataA.txt),
retrieved 2026-10-22. Across 70 categories, 1959-2019, the change in a category's price relative to all consumer
prices explained almost none of the change in its budget share: correlation -0.015 (95% bootstrap interval -0.27 to
0.28; permutation p = 0.90). An unchanged share is the case where quantity rises in proportion to the price fall
(elasticity of substitution about 1), the break-even case in chapter 1's rule. The spread is wide (implied
elasticity roughly 0.65 to 1.35). Weighted by spending (a check not pre-registered), the slope turns positive, +0.18
weighted by 1959 spending and +0.25 (interval 0.02 to 0.68) by 2019 spending: cheaper categories tended to lose some
share. The result is not evidence that demand was typically hungry. Quantities include BEA quality adjustment, and
share changes mix price and income effects.

**Note 12.**

> The economist James Bessen put it this way: "If demand increases sufficiently in response to productivity-improving technology, then employment will grow; otherwise, it will fall."

J. Bessen, "Automation and Jobs: When Technology Boosts Employment", *Economic Policy* (2019). Quoted from the April 2019 panel version. http://www.economic-policy.org/wp-content/uploads/2019/03/997_Automation-and-Jobs.pdf

**Note 13.**

> Three Stanford economists studying AI and jobs today, Erik Brynjolfsson and his colleagues Chandar and Chen, make the same point in more technical language: higher productivity in a job "could lead to either reduced or increased employment, depending on, among other things, how elastic demand is for the output of those workers."

Brynjolfsson, Chandar and Chen, "Canaries in the Coal Mine? Six Facts about the Recent Employment Effects of Artificial Intelligence", Stanford Digital Economy Lab, August 2026 update, footnote 2. https://digitaleconomy.stanford.edu/wp-content/uploads/2025/08/Canaries_BrynjolfssonChandarChen.pdf

**Note 14.**

> The economy as a whole grew too, but output per person in the whole economy rose only 30-fold over the same years.

Bessen (2019): "from 1810 to 2011, real GDP per capita rose 30-fold, but output per hour in cotton textiles rose over 800-fold."

**Note 15.**

> From then on, over the following decades, new machines came to cost jobs in those industries instead of adding them.

Bessen (2019): estimates of the elasticity of demand were "significantly greater than one" in the early years (1820 textiles, 1870 steel, 1910 cars) and "all are less than one" by 1950 (1951 for cars).

**Note 16.**

> In the near future, he writes, the main effect of automation may be "a major reallocation of jobs even if it does not permanently eliminate large numbers of jobs." And he adds: "This kind of change can be highly disruptive nevertheless."

Bessen (2019).

**Note 17.**

> Automation took about 0.7% a year, and new tasks added back only 0.35%.

D. Acemoglu and P. Restrepo, "Automation and New Tasks: How Technology Displaces and Reinstates Labor", *Journal of Economic Perspectives* 33(2), 2019. Figures from NBER Working Paper 25684 (2019). https://www.nber.org/system/files/working_papers/w25684/w25684.pdf

**Note 18.**

> Their answer was about 60%.

Autor, Chin, Salomons and Seegmiller, "New Frontiers: The Origins and Content of New Work, 1940–2018", NBER Working Paper 30389 (2022). https://www.nber.org/system/files/working_papers/w30389/w30389.pdf

**Note 19.**

> Since about 1980, they found, the pressure that removes old work has grown stronger, and the pull that creates new work has not.

Autor et al. (2022), conclusion: "the demand-eroding effects of automation innovations have intensified in the last four decades while the demand-increasing effects of augmentation innovations have not."

**Note 20.**

> Brynjolfsson, Chandar and Chen, working from the records of the payroll firm ADP, find "no evidence of widespread, economy-wide job displacement." In Denmark, where adoption surveys can be linked to official records, the economists Humlum and Vestergaard could rule out effects on pay or hours worked larger than 2%, two years after ChatGPT arrived.

Brynjolfsson, Chandar and Chen (August 2026 update), fact 1. A. Humlum and E. Vestergaard, "Still Waters, Rapid Currents: Early Labor Market Transformation under Generative AI", NBER Working Paper 33777 (revised March 2026). https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 21.**

> The authors call these early signals, "canaries in the coal mine", and they do not claim AI caused them.

Brynjolfsson, Chandar and Chen (August 2026 update), facts 2, 4 and 5. The 19% is the shortfall against the level employment would have reached had it kept pace with less-exposed peers.

**Note 22.**

> In jobs where people mainly use it as a helper, employment is flat or rising, and experienced workers do best.

Brynjolfsson, Chandar and Chen (August 2026 update), fact 5: losses are concentrated in jobs where AI is used mainly to automate tasks; where it is used mainly to augment work, employment is flat or rising. https://digitaleconomy.stanford.edu/app/uploads/2026/08/Canaries_August2026.pdf (added 2026-10-22 when the credit for this paragraph was restored).

**Note 23.**

> "If automation proceeds sufficiently slowly," they also write, "then there is always enough work for humans, and wages may rise forever."

A. Korinek and D. Suh, "Scenarios for the Transition to AGI", NBER Working Paper 32255 (2024). https://www.nber.org/system/files/working_papers/w32255/w32255.pdf

## Chapter 2: The Machine That Hired Tellers

**Note 1.**

> The actual count was about 506,000, half as many again.

US Bureau of Labor Statistics, *Monthly Labor Review*, July 1982, table 2: tellers 1980 about 506,000; BLS had projected 337,000 for 1980. https://www.bls.gov/opub/mlr/1982/07/art4full.pdf

**Note 2.**

> The census, which counts a little differently, put bank tellers at about 284,000 in 1970 and about 509,000 in 1980, a rise of nearly 80% in ten years.

US Census Bureau, 1980 Census, PC80-S1-15, table 1: bank tellers in the experienced civilian labor force, 284,413 (1970, recoded to 1980 occupations) and 509,449 (1980), up 79.1% (our calculation, `analysis/results.json`). This count includes the unemployed and is not comparable with the BLS figures. https://www.census.gov/content/dam/Census/library/publications/1984/demo/pc80-s1-15.pdf

**Note 3.**

> The first automated teller machines went into American banks in the 1970s,

J. Bessen, "Toil and Technology", IMF *Finance & Development* 52(1), March 2015. https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 4.**

> The first automated teller machines went into American banks in the 1970s, and by 1980 the country had about 19,000 of them.

Federal Reserve Bulletin (2009), "Households' Access to and Use of Electronic Banking", table 1 ("ATMs and bank branches", thousands). https://www.federalreserve.gov/Pubs/Bulletin/2009/articles/onlinebanking/dlink/fig1.htm

**Note 5.**

> By 2007 it stood at about 415,000, some 22 times the 1980 figure.

Federal Reserve Bulletin (2009), table 1: ATMs 1980 19,000; 1990 80,000; 1993 95,000; 2000 273,000; 2001 324,000; 2007 415,000. Yearly additions and the 22-fold rise are our calculations (`analysis/results.json`). https://www.federalreserve.gov/Pubs/Bulletin/2009/articles/onlinebanking/dlink/fig1.htm

**Note 6.**

> Bessen, whose rule chapter 1 quoted, puts the same turn in the mid-1990s, when banks began adding machines quickly.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 7.**

> The government's survey of jobs counted about 493,000 tellers in 2000 and about 608,000 in 2007.

BLS Occupational Employment Statistics, tellers (SOC 43-3071): 2000, 492,950; May 2007, 607,960. BLS warns that these surveys are not designed for comparisons over time; the counts cover wage and salary jobs. Series in `analysis/data/tellers.csv`, from Wayback Machine copies of https://www.bls.gov/oes/tables.htm

**Note 8.**

> Working from census samples, he found that "the number of bank teller jobs did not decrease as the ATMs were rolled out."

Bessen, "Toil and Technology" (2015), https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm . His teller series is built from census and American Community Survey samples: J. Bessen, Boston University School of Law Working Paper 15-49, working-paper version. https://www.bu.edu/law/files/2016/01/NewTech-012020161.pdf

**Note 9.**

> The staff of each branch shrank while the branches multiplied, and the teller's job held on.

Bessen, "Toil and Technology" (2015). The article gives 1988 to 2004 for the tellers per branch; the 43% follows in the same passage, with no separate dates. https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 10.**

> Bank branches numbered about 39,000 in 1980, about 51,000 by 1990, about 65,000 by 2000 and about 79,000 by 2007, on the Federal Reserve's count.

Federal Reserve Bulletin (2009), table 1: branches 1980 about 39,000; 1990 about 51,000; 2000 about 65,000; 2007 about 79,000. https://www.federalreserve.gov/Pubs/Bulletin/2009/articles/onlinebanking/dlink/fig1.htm

**Note 11.**

> The data, he writes, show "technology today largely displacing workers to new jobs, not replacing them entirely."

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 12.**

> Banks chasing market share wanted people at the counter who knew their customers and could sell them other services, and tellers joined what he calls the "relationship banking team."

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 13.**

> The skill that counted moved from the cash drawer to the conversation.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 14.**

> Tellers spent less time counting notes and more time with customers, moving toward selling and relationship work.

Bessen, "Toil and Technology" (2015), on tellers in the "relationship banking team"; and Bessen, BU School of Law Working Paper 15-49, working-paper version. https://www.bu.edu/law/files/2016/01/NewTech-012020161.pdf

**Note 15.**

> Bessen's book *Learning by Doing* (2015) makes a wider point that fits here: the skills a new technology calls for are often learned on the job, over years.

J. Bessen, *Learning by Doing: The Real Connection between Innovation, Wages, and Wealth* (Yale University Press, 2015), publisher's description. https://yalebooks.yale.edu/book/9780300195668/learning-by-doing/

**Note 16.**

> Branches were already multiplying before the machines arrived: on the FDIC's count of commercial-bank branches, they rose from about 22,000 in 1970 to about 38,000 in 1980, by close to 80%, when ATMs were still rare.

FDIC Historical Statistics on Banking, commercial-bank branches at year end: 21,597 (1970) and 38,458 (1980), +78.1% (our calculation, `analysis/results.json`). https://api.fdic.gov/banks/summary?filters=STNAME:%22U.S.%20States%20and%20DC%22

**Note 17.**

> By May 2025, about 329,000.

BLS Occupational Employment and Wage Statistics, tellers: May 2010, 556,310; May 2023, 340,820 (https://www.bls.gov/oes/2023/may/oes433071.htm); May 2025, 329,480 (BLS API). 2007 to 2025: about −46% (our calculation, `analysis/results.json`).

**Note 18.**

> Between 2007 and 2012, teller jobs fell by about 11%, while the number of commercial-bank branches still grew by about 6%.

Our calculation from `analysis/data/tellers.csv` (in `analysis/results.json`): OEWS tellers 607,960 (2007) to 541,770 (2012), −10.9%; FDIC commercial-bank branches 77,968 to 82,461, +5.8%; then a peak of 82,461 (2012) and 68,860 (2025), −16.5%. FDIC Historical Statistics on Banking, year-end. https://api.fdic.gov/banks/summary?filters=STNAME:%22U.S.%20States%20and%20DC%22

**Note 19.**

> On the FDIC's widest count, the offices run by all insured banks and savings institutions, the total peaked at about 99,500 in June 2009 and fell to just over 76,000 by June 2024, about a quarter fewer.

FDIC Summary of Deposits, offices operated by FDIC-insured institutions: 99,540 in June 2009, 86,364 in June 2019 (FDIC Quarterly 14(1), 2020, https://www.fdic.gov/analysis/quarterly-banking-profile/fdic-quarterly/2020-vol14-1/fdic-v14n1-4q2019-article.pdf); "more than 76,000" domestic offices in June 2024 (FDIC press release, 20 September 2024, https://www.fdic.gov/news/press-releases/2024/fdic-releases-results-summary-deposits-annual-survey). The fall of about 24% is our calculation.

**Note 20.**

> The steepest one-year drop in the survey, about 14%, came between 2020 and 2021, in the pandemic and in the years when the survey was moving to new job codes.

OEWS tellers 541,770 (2012) to 423,570 (May 2020), lower in every year between; 423,570 to 364,210 (May 2021), −14.0%, the largest one-year fall in the series (our calculation, `analysis/results.json`). OEWS moved to the 2018 occupation codes over May 2019 to 2021; the teller code did not change (`analysis/README.md`). https://www.bls.gov/oes/tables.htm

**Note 21.**

> Looking ahead, the Bureau of Labor Statistics names the forces it expects to keep cutting teller jobs: online and mobile banking, video kiosks, smarter ATMs, and fewer branches.

BLS *Occupational Outlook Handbook*, Tellers. https://www.bls.gov/ooh/office-and-administrative-support/tellers.htm

**Note 22.**

> Its projections use a slightly wider count, which puts 2025 at about 339,000.

BLS *Occupational Outlook Handbook*, Tellers: projected change 2025–35, −13% (−44,700 jobs from 339,200). The projections use the BLS National Employment Matrix, which also counts the self-employed, so 2025 differs from the OEWS figure. https://www.bls.gov/ooh/office-and-administrative-support/tellers.htm

**Note 23.**

> From 1990 to 2025, total employment in American commercial banks barely moved, staying between about 1.33 and 1.45 million people on annual averages.

BLS Current Employment Statistics, commercial banking employees (CEU5552211001), annual averages, 1990–2025: lowest 1,327,500 (2000), highest 1,450,800 (1990) (`analysis/results.json`). https://data.bls.gov/timeseries/CEU5552211001

**Note 24.**

> In the World Economic Forum's 2025 survey of employers, bank tellers are among the roles expected to shrink fastest by 2030.

World Economic Forum, *Future of Jobs Report 2025* (January 2025), employer survey, 2025–2030. https://reports.weforum.org/docs/WEF_Future_of_Jobs_Report_2025.pdf

**Note 25.**

> Half said they would move people from declining roles to growing ones, and 40% said they would cut staff.

World Economic Forum, *Future of Jobs Report 2025*: "50% planning to transition staff from declining to growing roles" and "40% planning to reduce staff as their skills become less relevant" (employer plans). https://reports.weforum.org/docs/WEF_Future_of_Jobs_Report_2025.pdf

**Note 26.**

> "It is not the 'brilliant' automation technologies that threaten employment and wages," they write, "but 'so-so technologies' that generate small productivity improvements." One of their examples is automated customer service, which they describe as "generally deemed to be low-quality."

D. Acemoglu and P. Restrepo, "Automation and New Tasks" (2019), NBER Working Paper 25684. https://www.nber.org/system/files/working_papers/w25684/w25684.pdf

**Note 27.**

> "'Brilliant' technologies will lead to declining employment if demand is inelastic," he writes, "and 'so-so' technologies can lead to job growth if demand is highly elastic."

J. Bessen, "Automation and Jobs: When Technology Boosts Employment" (2019), April 2019 panel version. http://www.economic-policy.org/wp-content/uploads/2019/03/997_Automation-and-Jobs.pdf

**Note 28.**

> Barcode scanners spread through American shops in the 1970s and 1980s, and one study found that early scanners raised a store's labour productivity by only about 4.5%, a modest gain.

E. Basker, "Raising the Barcode Scanner: Technology and Productivity in the Retail Sector", NBER Working Paper 17825, working-paper version (Census of Retail Trade, 1972, 1977 and 1982). https://www.nber.org/papers/w17825

**Note 29.**

> BLS counted about 3.29 million in 2000, and its job survey found about 3.64 million in 2018.

US Census Bureau, PC80-S1-15, table 1: cashiers 961,807 (1970) and 1,875,810 (1980), https://www.census.gov/content/dam/Census/library/publications/1984/demo/pc80-s1-15.pdf ; BLS, *The Economics Daily*, May 2003: 3.29 million in 2000, https://www.bls.gov/opub/ted/2003/may/wk3/art05.htm ; BLS OEWS, cashiers (SOC 41-2011), May 2018: 3,635,550, https://www.bls.gov/oes/2018/may/oes412011.htm

**Note 30.**

> Since 2018 the survey shows a fall, to about 3.09 million in 2025, about 15%, and BLS expects a further 6% drop by 2035, naming self-checkout among the reasons.

BLS OEWS, cashiers, May 2025: 3,089,410 (BLS API; −15% from 2018, our calculation); BLS *Occupational Outlook Handbook*, Cashiers: projected −6%, 2025–35. https://www.bls.gov/ooh/sales/cashiers.htm

**Note 31.**

> In a study chapter 5 looks at closely, Brynjolfsson, Li and Raymond gave 5,172 support agents an AI assistant instead, and issues resolved per hour rose by about 15%, while fewer of the newer agents left.

E. Brynjolfsson, D. Li and L. R. Raymond, "Generative AI at Work", *Quarterly Journal of Economics* 140(2), 2025. https://academic.oup.com/qje/article/140/2/889/7756313

## Chapter 3: Hungry Demand, and When It Fills

**Note 1.**

> In 1920, about one in every fifty American working women was a telephone operator.

J. Feigenbaum and D. P. Gross, "Answering the Call of Automation: How the Labor Market Adjusted to Mechanizing Telephone Operation", *Quarterly Journal of Economics* 139(3), 2024. Figures and quotations from NBER Working Paper 28061, working-paper version (revised February 2024), p. 6: operators were "roughly 2% of the U.S. female workforce" in 1920. https://www.nber.org/papers/w28061

**Note 2.**

> Each new subscriber added a whole set of new possible connections, and as the network grew, the number of operators needed to keep up with the calls swelled.

Feigenbaum and Gross (NBER w28061, 2024), p. 6. https://www.nber.org/papers/w28061

**Note 3.**

> AT&T, the dominant company, had become the largest employer in the country, and about half of its workforce were operators.

Feigenbaum and Gross (NBER w28061, 2024), pp. 5 and 7, citing their Appendix Table A.1: "nearly 15 million telephones" and "more than 65 million calls per day" in the 1920s; AT&T the largest US employer by the early 1920s, "with telephone operators comprising around half of its workforce." https://www.nber.org/papers/w28061

**Note 4.**

> Operators employed by the telephone companies grew from about 73,000 in 1910 to about 135,000 in 1920 and about 182,000 in 1930.

Feigenbaum and Gross (NBER w28061, 2024), table II: operators in the telephone industry (complete-count census), 1910, 73,030; 1920, 134,630; 1930, 182,040 (`analysis/data/telephone_operators.csv`). https://www.nber.org/papers/w28061

**Note 5.**

> Its own records reckoned that in the large cities, automatic switching could do away with up to 70 to 80% of the operators, and in 1917 its engineering department recommended it for local service there.

Feigenbaum and Gross (NBER w28061, 2024), p. 7, citing Gherardi (1917): AT&T records "projected that the automatic equipment would reduce the number of operators in large cities by up to 70 to 80%." https://www.nber.org/papers/w28061

**Note 6.**

> Once the first exchanges converted, in the late 1910s, the pace picked up: by 1930 about 32% of Bell telephones were on dial, and by 1940, 60%; in 1978 the last of them were converted.

Feigenbaum and Gross (NBER w28061, 2024), p. 7 and figure I (AT&T records): "Adoption began in the late 1910s and accelerated rapidly", 32% of Bell telephones on dial by 1930, 60% by 1940, the whole network by 1978. https://www.nber.org/papers/w28061

**Note 7.**

> Each turn of it sent a train of electrical pulses down the line, and the switching equipment read them and completed the circuit, with no one at a switchboard.

Feigenbaum and Gross (NBER w28061, 2024), p. 7. https://www.nber.org/papers/w28061

**Note 8.**

> The machines also had to be kept running, and the technicians who did that were mostly men.

Feigenbaum and Gross (NBER w28061, 2024), p. 7: "Mechanical switching specifically replaced operators in connecting local calls ... But even after automation, operators were still needed for long-distance calling, information and emergency services, and any remaining subscribers with manual service." Technicians "tended to be men." https://www.nber.org/papers/w28061

**Note 9.**

> In the cities the phone company switched over, the number of young women working as operators fell by 50% to 80%, and it stayed down.

Feigenbaum and Gross (NBER w28061, 2024), p. 1: after a cutover, the number of women aged 16 to 25 "in subsequent cohorts employed as telephone operators immediately and permanently fell by 50 to 80%" (estimated effect, 1910 to 1940). https://www.nber.org/papers/w28061

**Note 10.**

> The authors call it "a near-total collapse in entry-level hiring in one of the country's largest occupations for young women." With so many operators leaving and being replaced each year, they estimate it may have shut off a first job for "as much as 10 to 15% of peak cohorts" of young women.

Feigenbaum and Gross (NBER w28061, 2024), pp. 1 and 27. Turnover ran at up to 40% a year (p. 6). https://www.nber.org/papers/w28061

**Note 11.**

> Those who kept working were much more likely to have changed careers, and on average they moved into lower-paid kinds of work: on a standard measure of what an occupation pays, they slipped about 5% while their peers rose about 8%.

Feigenbaum and Gross (NBER w28061, 2024), pp. 19 and 20, tables V and VI: compared with matched women in cities without a cutover; continuing workers about 11 percentage points (close to 40%) more likely to switch careers; occupation score (an income proxy) down 5% against peers' rise of 8%. https://www.nber.org/papers/w28061

**Note 12.**

> But telephone operation was "one of the few opportunities for women with the potential to be a career," they write, and its loss "was costly for those who would have chosen to keep them."

Feigenbaum and Gross (NBER w28061, 2024), p. 3. https://www.nber.org/papers/w28061

**Note 13.**

> Office jobs such as typist and secretary took many of them in, and lower-paid work such as food service took others.

Feigenbaum and Gross (NBER w28061, 2024), p. 1: "jobs with similar demographics and wages (such as typists and secretaries), and some with lower wages (such as food service workers)"; "wage data for this era are more limited." https://www.nber.org/papers/w28061

**Note 14.**

> Demand for that work grew to absorb them, the authors find, and it did so fairly quickly.

Feigenbaum and Gross (NBER w28061, 2024), p. 27. https://www.nber.org/papers/w28061

**Note 15.**

> Cutovers to dial were typically accompanied by telephone rate increases: AT&T "did not pass through its cost savings." The time the dial saved its users was small too, by their estimate less than an hour and a half a year for a business telephone.

Feigenbaum and Gross (NBER w28061, 2024), p. 24 and Appendix E.2.2: "annual time savings of less than 1.5 hours per business telephone." https://www.nber.org/papers/w28061

**Note 16.**

> Over the same years, operators working for other employers, at the private switchboards of large firms, hospitals and hotels, grew from about 23,000 to about 41,000.

Feigenbaum and Gross (NBER w28061, 2024), table II: telephone industry 1940, 152,700; operators in other industries 1930, 22,830, and 1940, 41,170; p. 6, note 5, on private switchboards at "large firms, hospitals, hotels." https://www.nber.org/papers/w28061

**Note 17.**

> The 1980 census put them at about 306,000.

US Census Bureau, 1980 Census, PC80-S1-15, table 1: telephone operators in the experienced civilian labor force, 408,560 (1970, recoded to 1980 occupations) and 306,360 (1980). This count includes the unemployed and is not comparable with the other series. https://www.census.gov/content/dam/Census/library/publications/1984/demo/pc80-s1-15.pdf

**Note 18.**

> By 2025 the total was about 38,000, a fall of 87%.

BLS Occupational Employment Statistics, switchboard operators, including answering service (SOC 43-2011), and telephone operators (43-2021): 2000, 243,100 and 52,150 (295,250 together); May 2025, 34,280 and 3,430 (37,710). The fall of 87.2% is our calculation (`analysis/results.json`). BLS warns that these surveys are not designed for comparisons over time; the counts cover wage and salary jobs. Wayback Machine copies of https://www.bls.gov/oes/tables.htm

**Note 19.**

> Callers still wanted a person to talk to, and in his account receptionists became that person, so their jobs grew while switchboard jobs shrank.

J. Bessen, "Toil and Technology", IMF *Finance & Development* 52(1), March 2015. https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 20.**

> It reached American textile manufacture in 1814,

J. Bessen, "Automation and Jobs: When Technology Boosts Employment", Boston University School of Law, Law & Economics Paper No. 17-09 (12 April 2017), p. 8. An earlier version of the paper cited in chapter 1. https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 21.**

> Factory weaving jobs grew all the same.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 22.**

> On Bessen's account, competition between the mills turned the labour saved into cheaper cloth, and cheaper cloth sold in such quantity that the extra yards needed more weavers than the machines had saved.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 23.**

> During the nineteenth century, by his estimate, American cotton textiles saw labour productivity rise nearly 30-fold, while consumption of cotton cloth rose 100-fold.

Bessen, "Automation and Jobs" (April 2017), p. 6. https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 24.**

> That is the price side of the 800-fold rise in output per hour that chapter 1 reported.

Bessen, "Automation and Jobs" (April 2017), p. 8: "From 1810 to 2011 ... output per hour in cotton textiles rose over 800-fold; inflation-adjusted prices correspondingly fell by three orders of magnitude." https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 25.**

> It rose sharply only once the skills the new machines needed, and the training for them, had become standard.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 26.**

> By the late nineteenth century weavers' pay was rising well ahead of other workers'.

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 27.**

> Bessen's abstract puts it in three words: "Markets became saturated."

Bessen, "Automation and Jobs" (April 2017), abstract. Chapter 1's source, the 2019 version, finds demand elasticities below one in all three industries by about 1950. https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 28.**

> In his table, production workers in American cotton and synthetic textiles, weavers among them, numbered about 350,000 in 1950, about 120,000 in 1995 and about 16,000 in 2011.

Bessen, "Automation and Jobs" (April 2017), table on p. 28: production workers, "Cotton & synthetic textiles", actual, in thousands. His note 1 defines the industry as broadwoven fabrics of cotton and manmade fibres (SIC 2211 and 2221). The 95% and the 334,000 follow from his figures. https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 29.**

> Import penetration in textiles, by his measure, was only about 9% in 2005.

Bessen, "Automation and Jobs" (April 2017), pp. 28 and 29, and table on p. 28 (technology share 71% for 1950 to 2011, 35% for 1995 to 2011); import penetration in textiles 8.9% in 2005. https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 30.**

> Its production jobs fell from about 550,000 in 1950 to about 100,000 in 2011, and he attributes about 80% of that loss to productivity.

Bessen, "Automation and Jobs" (April 2017), p. 28 (steel, technology share 80%). https://www.bu.edu/law/files/2017/04/autogro.pdf

**Note 31.**

> By 1945 there were about 2.4 million tractors, and by 1960 about 4.7 million.

USDA Economic Research Service, *The 20th Century Transformation of U.S. Agriculture and Farm Policy*, EIB-3 (2005): tractors, horses and mules; agriculture's share of the workforce in 1930. https://www.ers.usda.gov/media/8254/eib-3.pdf

**Note 32.**

> Farm output in 2023 was about three times what it was in 1948.

USDA Economic Research Service, Agricultural Productivity in the United States, summary of recent findings. https://www.ers.usda.gov/data-products/agricultural-productivity-in-the-united-states/summary-of-recent-findings

**Note 33.**

> By 1945 it was about 16%, and by 1970 about 4%.

USDA ERS, EIB-3 (2005): 41% (1900), 16% (1945), 4% (1970). The bases differ by year (workforce, labor force, employed labor force). https://www.ers.usda.gov/media/8254/eib-3.pdf

**Note 34.**

> By 2024, about 1.4% of employed Americans worked in agriculture and related industries.

BLS Current Population Survey, employed in agriculture and related industries (LNU02034560) as a share of all employed (LNU02000000), 2024 annual average. Our calculation (`analysis/results.json`); this series is not joined to the ERS figures. https://data.bls.gov/timeseries/LNU02034560

**Note 35.**

> The government's household survey put about 7.6 million Americans in agriculture and related industries in 1948 and about 2.3 million in 2024, a fall of about 70%.

BLS Current Population Survey, LNU02034560, annual averages: 7,628,600 (1948) and 2,254,100 (2024), −70.5% (our calculation, `analysis/results.json`). The series breaks in 2003, when its industry codes changed. https://data.bls.gov/timeseries/LNU02034560

**Note 36.**

> In the department's words, "mechanization contributed to rising agricultural productivity, thereby reducing the need for labor." Since 1990, its figures have held roughly steady.

USDA Economic Research Service, Farm Labor (from the NASS Farm Labor Survey): self-employed and family farmworkers 7.60 million (1950) and 2.06 million (2000); hired farmworkers 2.33 million and 1.13 million. https://www.ers.usda.gov/topics/farm-economy/farm-labor

**Note 37.**

> Bessen notes only that "as agricultural jobs disappeared, new jobs arose in the manufacturing and service sectors."

Bessen, "Toil and Technology" (2015). https://www.imf.org/external/pubs/ft/fandd/2015/03/bessen.htm

**Note 38.**

> In Bessen's summary of that standard account, as nations grow richer, demand for farm and factory goods falls relative to everything else, and "with labor productivity growth, relative employment in these sectors falls even faster."

Bessen, "Automation and Jobs" (April 2017), pp. 6 and 7, summarising Engel (1857) and Clark (1940). https://www.bu.edu/law/files/2017/04/autogro.pdf

## Chapter 4: Knowledge Work's Tests

**Note 1.**

> It was the first electronic spreadsheet for a personal computer, and it was so useful to people who worked with numbers that, as a 2015 radio programme put it, it was "the $99 piece of software that makes people go out and buy the $2,000 computer."

NPR *Planet Money*, Episode 606, 25 February 2015 (transcript), host Jacob Goldstein. https://text.npr.org/389027988

**Note 2.**

> Running all the numbers again, the host summed up, could take a whole day, "a really boring day".

NPR *Planet Money*, Episode 606 (2015): Allen Sneider's words; "a really boring day" is host David Kestenbaum's summary of his account. https://text.npr.org/389027988

**Note 3.**

> Bookkeepers went from about 1,705,000 to about 1,895,000 over the same ten years.

US Census Bureau, 1980 Census, PC80-S1-15, table 1: accountants and auditors in the experienced civilian labor force, 646,490 (1970, recoded to 1980 occupations) and 1,012,857 (1980); bookkeepers 1,704,744 and 1,895,473. This count includes the unemployed and is not comparable with the BLS payroll figures (`analysis/results.json`). https://www.census.gov/content/dam/Census/library/publications/1984/demo/pc80-s1-15.pdf

**Note 4.**

> Taken together, the two jobs grew by about 77%.

BLS Occupational Employment and Wage Statistics (OEWS): accountants and auditors (SOC 13-2011) 863,320 (2000), 1,449,500 (May 2025), +67.9%; financial analysts (13-2051) 159,490 and 361,980; the two together +77.1% (our calculation, `analysis/results.json`). BLS warns that these surveys are not designed for comparisons over time; the counts cover wage and salary jobs. Wayback Machine copies of https://www.bls.gov/oes/tables.htm

**Note 5.**

> On the old definition, the rise would probably have been larger.

BLS OEWS: financial analysts (13-2051) 306,200 (2018), 291,880 (2021); financial risk specialists (13-2054) 54,320 (2021). OEWS phased in the 2018 occupation codes over May 2019 to 2021; analysts are not published for 2019 and 2020 (`analysis/README.md`). https://www.bls.gov/oes/tables.htm

**Note 6.**

> Then they fell, from the recession year of 2009 on, to about 1,374,000 by May 2025, a drop of about 26%.

> The clerks' count never returned to its old level.

BLS OEWS, bookkeeping, accounting and auditing clerks (43-3031): 1,858,500 (May 2007), 1,855,010 (2008), 1,757,870 (2009), 1,373,680 (May 2025), −26.1% from 2007 (our calculation, `analysis/results.json`). Accountants and auditors (13-2011): 1,133,580 (2008), 1,072,490 (2010). https://www.bls.gov/oes/tables.htm

**Note 7.**

> It came into wide use, two economists at the University of Oxford argue, only in 2010, when Google released it as a phone app and built it into its Chrome browser.

C. B. Frey and P. Llanos-Paredes, "Lost in Translation: Artificial Intelligence and the Demand for Foreign Language Skills", Oxford Internet Institute and Oxford Martin School, version of 7 March 2025, p. 2. https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

**Note 8.**

> Google moved its service to neural networks in 2016, and ChatGPT brought large language models to the public at the end of 2022.

Google Research blog, "A Neural Network for Machine Translation, at Production Scale", 27 September 2016, https://research.google/blog/a-neural-network-for-machine-translation-at-production-scale/ ; OpenAI, "Introducing ChatGPT", 30 November 2022, https://openai.com/index/chatgpt/

**Note 9.**

> In 2026, Google's published price for its language-model translation works out to roughly a hundredth of a cent per word, by our calculation from its rates.

Google Cloud Translation pricing (fetched 21 October 2026): Translation LLM, $10 per million input characters and $10 per million output characters; about $0.00012 per word at six characters a word (our calculation). https://cloud.google.com/translate/pricing

**Note 10.**

> Its AI tool, GCtranslate, launched in June 2025 for use across the federal public service, had translated about 380 million words by the end of June 2026.

Translation Bureau, Government of Canada, "Data and facts 2025 to 2026": 683 translators, "including active and nonactive translators", plus managers who don't translate, and about 253 million words, both for 1 April 2025 to 31 March 2026; about 380 million words translated by GCtranslate (launched 10 June 2025) as of 30 June 2026. https://www.canada.ca/en/translation-bureau/about/data-facts/2025-2026.html

**Note 11.**

> Instead, American employers' count of interpreters and translators (the official figures don't separate them) grew from about 16,800 in 2000 to a peak of about 58,900 in 2019, three and a half times as many.

BLS OEWS, interpreters and translators (27-3091): 16,780 (2000); 58,870 (May 2019), 3.51 times (our calculation, `analysis/results.json`). https://www.bls.gov/oes/2019/may/oes273091.htm

**Note 12.**

> In May 2025 it stood at about 52,100, some 12% below the peak.

BLS OEWS, interpreters and translators: 56,920 (2020), 52,170 (2021), 52,160 (2022), 51,560 (2023), 53,360 (2024), 52,060 (May 2025); −11.6% from 2019, −0.2% from 2021 (our calculation, `analysis/results.json`). https://www.bls.gov/oes/tables.htm

**Note 13.**

> In all, they put the cost at about 28,000 translator jobs that would otherwise have been created.

Frey and Llanos-Paredes (March 2025), pp. 3 and 15: Google Trends searches as the measure of use; "approximately 28,000 fewer translator positions were created". https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

**Note 14.**

> They also lump in interpreters, who are less exposed to machine translation, and the inclusion of interpreters, the authors write, "likely dilutes" the effect.

Frey and Llanos-Paredes (March 2025), p. 11: OEWS "excludes about 21 percent of translators and interpreters that are self-employed"; "interpreters are less likely to be affected by machine translation". https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

**Note 15.**

> The machine also cut demand for language skills in other jobs: postings asking for Spanish or Chinese grew more slowly too.

Frey and Llanos-Paredes (March 2025), p. 4: job postings from Lightcast, 2010 to 2023; placebo occupations (editors, proofreaders, technical writers, desktop publishers) show "no impact"; demand for Spanish and Chinese skills fell (-1.4 and -1.3 percentage points of posting growth). https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

**Note 16.**

> In the same study, translators' wage growth slowed while Google Translate was new, and began to recover around 2016, leaving no clear effect over the whole period.

Frey and Llanos-Paredes (March 2025), pp. 3 and 15: wage growth "slowed" and "began to recover around 2016, resulting in no statistically significant impact on wages over the full sample period." https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

**Note 17.**

> Prices rose about 25% over those six years, so after inflation the average fell by about 7%.

BLS OEWS, interpreters and translators, mean annual wage: $57,000 (May 2019) and $66,360 (May 2025, national file `oesm25nat`), +16.4%. BLS consumer price index for all urban consumers (CUUR0000SA0): 256.092 (May 2019), 321.465 (May 2025), +25.5%. Real change −7.3% (our calculation). https://www.bls.gov/oes/2019/may/oes273091.htm ; https://data.bls.gov/timeseries/CUUR0000SA0

**Note 18.**

> More than three-quarters expected it to cut their future income.

Society of Authors, "SoA survey reveals a third of translators and quarter of illustrators losing work to AI", 11 April 2024 (read from a Wayback Machine copy): survey of members and other authors, January 2024, "nearly 800 responses"; translators: 36% lost work, 43% income "decreased in value", 37% had used generative AI in their work, 8% because a "publisher or commissioning organisation" asked, 77% expect lower future income; the number of translators who answered is not given. https://www2.societyofauthors.org/2024/04/11/soa-survey-reveals-a-third-of-translators-and-quarter-of-illustrators-losing-work-to-ai/ Also European Writers' Council, 9 May 2024 (787 responses). https://europeanwriterscouncil.eu/soa-survey-uk-ai-2024/

**Note 19.**

> The Bureau of Labor Statistics, counting the self-employed too, puts the total at about 73,900 in 2025, and projects a rise of 2% by 2035.

BLS *Occupational Outlook Handbook*, Interpreters and Translators (2025), including the self-employed. https://www.bls.gov/ooh/media-and-communication/interpreters-and-translators.htm

**Note 20.**

> In 2016, at a conference in Toronto, the AI pioneer Geoffrey Hinton said that "people should stop training radiologists now".

> Deena Mousa, who wrote about the field for *Works in Progress* in 2025, put the stakes plainly: "If the most extreme predictions about the effect of AI on employment and wages were true, then radiology should be the canary in the coal mine."

Creative Destruction Lab, "Geoff Hinton: On Radiology", recorded at the 2016 Machine Learning and the Market for Intelligence conference in Toronto, posted 24 November 2016, https://www.youtube.com/watch?v=2HMPRXstSvQ ; words as quoted in D. Mousa, "The Algorithm Will See You Now", *Works in Progress*, 25 September 2025. https://worksinprogress.co/issue/the-algorithm-will-see-you-now/

**Note 21.**

> The US Food and Drug Administration had cleared 26 AI tools for radiology by 2016, and 1,095 by 2025.

US FDA, list of AI-enabled medical devices, lead panel Radiology, cumulative by decision year (our calculation, `analysis/results.json`). https://www.fda.gov/medical-devices/artificial-intelligence-enabled-medical-devices/list-artificial-intelligence-enabled-medical-devices

**Note 22.**

> Diagnostic radiology filled 996 of its 997 places in 2022, 99.9%, and 1,042 of 1,057 in 2025, 98.6%.

AuntMinnie.com staff, "Diagnostic radiology positions fall short of 100% filled", 24 March 2025 (NRMP Main Residency Match, PGY-2 positions). https://www.auntminnie.com/radiology-education/article/15741177/diagnostic-radiology-positions-fall-short-of-100-filled

**Note 23.**

> She put radiologists' average income that year at about $520,000, 48% more than in 2015, with vacancies at record highs.

Mousa (2025): "a record 1,208 positions across all radiology specialties", "an average income of $520,000, over 48 percent higher than the average salary in 2015", vacancy rates "at all-time highs". https://worksinprogress.co/issue/the-algorithm-will-see-you-now/

**Note 24.**

> At the Mayo Clinic, the *New York Times* reported in a story TechCrunch picked up, the number of radiologists had grown by about 55% since Hinton's remark.

*New York Times* (S. Lohr, 14 May 2025), as reported by TechCrunch, 14 May 2025. https://techcrunch.com/2025/05/14/radiologists-arent-going-anywhere/

**Note 25.**

> As Mousa puts it, "Without malpractice coverage, hospitals cannot afford to let algorithms sign reports."

Mousa (2025): "models often don't work as well outside of their test conditions"; regulators and insurers "reluctant to approve or cover fully autonomous radiology models"; stroke, breast cancer and lung cancer "account for about 60 percent of models, but only a minority of the actual radiology imaging volume"; the insurer Berkley's "Absolute AI Exclusion"; the 2012 study, "only 36 percent of their time was dedicated to direct image interpretation." https://worksinprogress.co/issue/the-algorithm-will-see-you-now/

**Note 26.**

> "For now," Mousa writes, "usage is too sparse to make a difference."

Mousa (2025), citing a 2024 investigation and a 2025 survey. https://worksinprogress.co/issue/the-algorithm-will-see-you-now/

**Note 27.**

> Mousa sees Jevons at work here.

Mousa (2025): the Vancouver General study and the utilization rate "per 1,000 insured patients", 2000 to 2008. https://worksinprogress.co/issue/the-algorithm-will-see-you-now/

**Note 28.**

> The change from 2021 is within it.

BLS OEWS, radiologists (29-1224): 29,530 (2021), 29,250 (2022), 31,960 (2023), 26,290 (2024), 26,770 (May 2025). Using 1.96 times the published relative standard errors, the 2023 to 2025 fall (5,190) exceeds the combined margin (about 5,030); the 2021 to 2025 change does not. A rough test (our calculation, `analysis/results.json`). https://www.bls.gov/oes/tables.htm

**Note 29.**

> Radiologists' average pay on payrolls went from about $301,700 in 2021 to about $381,500 in 2025, about 26% more, or about 6% after inflation.

BLS OEWS, radiologists, mean annual wage: $301,720 (May 2021), $381,530 (May 2025, national file `oesm25nat`), +26.5%; CPI-U (CUUR0000SA0) 269.195 (May 2021) and 321.465 (May 2025), +19.4%; real change +5.9% (our calculation). https://www.bls.gov/oes/2021/may/oes291224.htm ; https://data.bls.gov/timeseries/CUUR0000SA0

**Note 30.**

> Frey and Llanos-Paredes offer one explanation for the recovery in translators' pay: a gradual shift toward harder translation that machines handle less well, which took firms and translators time.

Frey and Llanos-Paredes (March 2025), pp. 15 and 16: "a gradual compositional shift toward higher-skill translation tasks that are less susceptible to automation"; "Both firms and translators may have required some time to adjust." https://oms-www.files.svdcdn.com/production/downloads/academic/Frey_LlanosParedes_2025_LostInTranslation.pdf

## Chapter 5: What the AI Studies Say Now

**Note 1.**

> Three economists, Brynjolfsson, Li and Raymond, studied their records.

E. Brynjolfsson, D. Li and L. R. Raymond, "Generative AI at Work", *Quarterly Journal of Economics* 140(2), May 2025, abstract (read via Crossref, 21 October 2026). https://academic.oup.com/qje/article/140/2/889/7756313

**Note 2.**

> The headline result was an average rise in productivity of 15%, measured as customer issues resolved per hour.

Brynjolfsson, Li and Raymond (2025), abstract: "by 15% on average". https://academic.oup.com/qje/article/140/2/889/7756313

**Note 3.**

> At the top, the most experienced and skilled agents went a little faster, and the quality of their work slipped slightly.

Brynjolfsson, Li and Raymond, arXiv 2304.11771 v2 (November 2024), the authors' version of the published paper: "approximate increase of 30%" for less skilled and less experienced agents; "a 0.5 increase or 36% increase in resolutions per hour" for the lowest skill quintile. Most experienced agents: QJE abstract. https://arxiv.org/pdf/2304.11771

**Note 4.**

> Customers changed too: with the assistant in use, they were politer to agents and asked less often to be put through to a manager.

Brynjolfsson, Li and Raymond (2025): "a decrease in worker attrition, which is driven by the retention of newer workers"; "60% of agents in contact centers leave each year" is industry context quoted in the paper; customers "more polite and less likely to ask to speak to a manager" (abstract). https://academic.oup.com/qje/article/140/2/889/7756313

**Note 5.**

> The published paper also reports evidence that it "facilitates worker learning and improves English fluency, particularly among international agents."

Brynjolfsson, Li and Raymond (2025), abstract: AI assistance "facilitates worker learning and improves English fluency, particularly among international agents"; gains "largest for moderately rare problems, where human agents have less baseline experience but the system still has adequate training data". https://academic.oup.com/qje/article/140/2/889/7756313

**Note 6.**

> Two weeks later, people who had used the tool in the experiment were twice as likely to say they used it at work, and two months later 1.6 times as likely.

S. Noy and W. Zhang, "Experimental evidence on the productivity effects of generative artificial intelligence", *Science* 381(6654), 2023, abstract: "midlevel professional writing tasks", "a preregistered online experiment", "occupation-specific, incentivized writing tasks". https://pubmed.ncbi.nlm.nih.gov/37440646/

**Note 7.**

> Again, "less experienced developers had higher adoption rates and greater productivity gains."

Cui, Demirer, Jaffe, Musolff, Peng and Salz, "The Effects of Generative AI on High-Skilled Work: Evidence from Three Field Experiments with Software Developers", *Management Science*, 2026 (doi 10.1287/mnsc.2025.00535): "a 26.08% increase (standard error: 10.3%) in completed tasks". The third firm is an anonymous Fortune 100 company. https://www.microsoft.com/en-us/research/publication/the-effects-of-generative-ai-on-high-skilled-work-evidence-from-three-field-experiments-with-software-developers/

**Note 8.**

> One self-contained task in a lab is a narrow test, which is why the field experiments carry more weight.

Peng, Kalliamvakou, Cihon and Demirer, "The Impact of AI on Developer Productivity: Evidence from GitHub Copilot", arXiv 2302.06590, February 2023: "completed the task 55.8% faster (95% confidence interval: 21-89%)"; tests run May to June 2022. https://arxiv.org/pdf/2302.06590

**Note 9.**

> Experts asked in advance had been further off still: economists predicted the tasks would take 39% less time, and machine-learning researchers 38% less.

Becker, Rush, Barnes and Rein (METR), "Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity", arXiv 2507.09089, July 2025, abstract: AI tools "at the February-June 2025 frontier"; each task "randomly assigned to allow or disallow usage of early 2025 AI tools"; expert predictions "economics (39% shorter) and ML (38% shorter)". https://arxiv.org/pdf/2507.09089

**Note 10.**

> The authors were careful to add that they "do not make predictions about the development or adoption timeline."

Eloundou, Manning, Mishkin and Rock, "GPTs are GPTs", arXiv 2303.10130 v5 (August 2023), the source of the quotes; published in shorter form in *Science* 384(6702), 2024. The 15% and 47% to 56% figures are from the same version. https://arxiv.org/pdf/2303.10130

**Note 11.**

> "For the other half, AI applications may execute key tasks currently performed by humans, which could lower labor demand, leading to lower wages and reduced hiring. In the most extreme cases, some of these jobs may disappear."

K. Georgieva, "AI Will Transform the Global Economy. Let's Make Sure It Benefits Humanity", IMF blog, 14 January 2024, summarising IMF Staff Discussion Note SDN/2024/001. Wording checked on a 2024 Internet Archive copy of the page, 21 October 2026. https://www.imf.org/en/Blogs/Articles/2024/01/14/ai-will-transform-the-global-economy-lets-make-sure-it-benefits-humanity

**Note 12.**

> On its count, roughly 36% of occupations were using AI for at least a quarter of their tasks.

Anthropic, "The Anthropic Economic Index", 10 February 2025: usage on Claude.ai. https://www.anthropic.com/news/the-anthropic-economic-index

**Note 13.**

> Employers, the two economists write, "absorb AI through task reorganization," including "new tasks in content generation, AI oversight, and AI integration."

A. Humlum and E. Vestergaard, "Still Waters, Rapid Currents: Early Labor Market Transformation under Generative AI", NBER Working Paper 33777 (revised March 2026): "precise null effects on earnings and recorded hours at both the worker and workplace levels, ruling out effects larger than 2% two years after the launch of ChatGPT". https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 14.**

> About 26.6% of AI users said they used it at least in part to replace tasks workers had done, and nearly 85% of those said it replaced only a small number.

Bonney et al., "Tracking Firm Use of AI in Real Time: A Snapshot from the Business Trends and Outlook Survey", NBER Working Paper 32319, April 2024 (Census Bureau survey, September 2023 to February 2024; shares of AI-using firms). https://www.nber.org/system/files/working_papers/w32319/w32319.pdf

**Note 15.**

> Larger companies expected to shed workers, and smaller ones expected modest growth.

Baslandze et al., "Artificial Intelligence, Productivity, and the Workforce: Evidence from Corporate Executives", NBER Working Paper 34984, March 2026: "firm-size-and-sector-weighted aggregate employment is expected to decline by less than 0.4% due to AI in 2026". https://www.nber.org/system/files/working_papers/w34984/w34984.pdf

**Note 16.**

> When the image generators DALL-E 2 and Midjourney arrived in 2022, freelancers in design and image work saw similar losses.

> The authors found "suggestive evidence that top freelancers are disproportionately affected by AI."

> The authors take this to mean that, in the short term, generative AI "reduces overall demand for knowledge workers of all types."

X. Hui, O. Reshef and L. Zhou, "The Short-Term Effects of Generative Artificial Intelligence on Employment: Evidence from an Online Labor Market", SSRN working paper, 31 July 2023 (published in *Organization Science*, 2024); all figures and quotes from the working paper. https://www.enriquedans.com/wp-content/uploads/2023/11/Short-Term-Effects-of-Generative-AI-Employment-SSRN.pdf

**Note 17.**

> Between November 2022 and June 2026, employment of 22- to 25-year-olds in the two most AI-exposed fifths of occupations fell about 11%, while the same age group grew by about 10% in the three fifths least exposed.

Brynjolfsson, Chandar and Chen, "Canaries in the Coal Mine? Six Facts about the Recent Employment Effects of Artificial Intelligence", Stanford Digital Economy Lab, August 2026 update. The 81% is our calculation from the two levels (0.89 / 1.10), and matches the authors' 19% kept-pace shortfall. https://digitaleconomy.stanford.edu/wp-content/uploads/2025/08/Canaries_BrynjolfssonChandarChen.pdf

**Note 18.**

> And part of the gap fades once occupations' education levels are allowed for, which could mean education explains it, or that education is the route AI works through.

Brynjolfsson, Chandar and Chen (August 2026 update): abstract (facts 3 and 6, caveats); introduction (15% at the July 2025 data vintage, 19% as of June 2026; the earlier 13% and 16% regression estimates; widening "long after interest rates peaked"); Online Appendix section L (the most exposed quintile's within-firm estimate "is no longer statistically significant"). https://digitaleconomy.stanford.edu/wp-content/uploads/2025/08/Canaries_BrynjolfssonChandarChen.pdf

**Note 19.**

> From May 2022 to May 2025, the fifth of occupations most exposed to AI grew about as fast as the least exposed fifth: 0.45 percentage points a year faster, with a 95% interval running from 0.97 slower to 1.87 faster, against a gap of 0.02 before ChatGPT.

Our calculation, pre-registered test T4 (exposure), code in `analysis/part3/t4_t5/`, results in
`analysis/results_part3_t4_t5.json`, red-team checks in `analysis/part3/redteam/rt_t4_t5.py` (REDTEAM.md, T4). Data:
BLS, Occupational Employment and Wage Statistics, national estimates, May 2016, 2019, 2022 and 2025 (Wayback Machine
copies of bls.gov files, e.g.
https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip), occupations
joined across SOC 2010 and 2018 with the BLS crosswalk
(https://web.archive.org/web/20201016183750id_/https://www.bls.gov/soc/2018/soc_2010_to_2018_crosswalk.xlsx); 762
occupation units split into fifths by exposure. Exposure: Eloundou, Manning, Mishkin and Rock, "GPTs are GPTs: An
Early Look at the Labor Market Impact Potential of Large Language Models", arXiv:2303.10130 (v5), human-rated beta
score, from https://github.com/openai/GPTs-are-GPTs (MIT License, Copyright (c) 2024 OpenAI). Growth is employment
growth per year of each fifth; the effect is top minus bottom fifth, 2022-2025, +0.45 points a year (95% bootstrap
interval -0.97 to +1.87); placebo 2016-2019, +0.02. The interval rules out a shortfall of more than about 1 point a
year; smaller effects cannot be seen. Caveats: exposure measures what LLMs could do, rated in 2023, not use; OEWS May
estimates pool three years of survey panels and all ages, so the young-worker gap found by Brynjolfsson, Chandar and
Chen in ADP payroll data would not show here.

**Note 20.**

> Raising low-skill workers' productivity at some tasks may still widen inequality, he shows in theory, if AI creates no new tasks for them.

D. Acemoglu, "The Simple Macroeconomics of AI", NBER Working Paper 32487, May 2024: "no more than a 0.66% increase in total factor productivity (TFP) over 10 years", "less than 0.53%" with hard-to-learn tasks; "even when AI improves the productivity of low-skill workers in certain tasks (without creating new tasks for them), this may increase rather than reduce inequality." https://www.nber.org/system/files/working_papers/w32487/w32487.pdf

## Chapter 6: Find Your Hungry Demand

**Note 1.**

> As reported by the Irish tech site TechCentral, Amazon said that for every e-book copy sold at $14.99, it would sell 1.74 copies at $9.99.

Amazon statement during the Hachette dispute, as reported by TechCentral.ie, 30 July 2014 ("Tuesday", hence 29 July), paraphrasing Amazon: e-books at $9.99 "will boost sales by over 74%", with "estimates of the price-elasticity of e-books ... based on repeated measurements across many titles". Amazon's original post was not reached. https://www.techcentral.ie/amazon-says-e-books-will-make-more-money-for-publishers

**Note 2.**

> That is a price a third lower and revenue about 16% higher.

TechCentral.ie (2014), Amazon's example: 100,000 copies at $14.99 against 174,000 at $9.99. The 33% price fall and 16% revenue rise ($1,499,000 against $1,738,000) are our calculation. The one-and-a-half-times break-even in the next section is also ours ($14.99 ÷ $9.99 ≈ 1.50). https://www.techcentral.ie/amazon-says-e-books-will-make-more-money-for-publishers

**Note 3.**

> The average elasticity was about −1.76.

Tellis, "The Price Elasticity of Selective Demand: A Meta-Analysis of Sales Response Models", Marketing Science Institute working paper, 1988, Main Findings: 367 models, more than 220 brands or markets, uncorrected mean −1.76, for brand sales or market share. https://www.msi.org/working-papers/the-price-elasticity-of-selective-demand-a-metaanalysis-of-sales-response-models/

**Note 4.**

> They found demand "quite inelastic." Most of their estimates fell between −0.4 and −0.6, with −0.55 for the whole sample and −0.33 in Los Angeles.

Cohen, Hahn, Hall, Levitt and Metcalfe, NBER Working Paper 22627, September 2016 (working-paper version): about 50 million UberX sessions, first 24 weeks of 2015, the four largest US cities; regression-discontinuity design on surge pricing; whole-sample elasticity −0.55 (standard error 0.02), most estimates −0.4 to −0.6, Los Angeles −0.33; the authors describe demand as "quite inelastic". The 10%-to-5% illustration is our rounding. https://www.nber.org/papers/w22627

**Note 5.**

> The economists Dubé and Misra ran such a test at what their paper calls "a large, digital firm." The paper's acknowledgements thank ZipRecruiter, and Misra was a contracted adviser to the firm.

Dubé and Misra, NBER Working Paper 23775, September 2017, revised June 2021 (working-paper version); published in *Journal of Political Economy* 131(1), 2023. The paper calls the firm "a large, digital firm"; ZipRecruiter is thanked in the acknowledgements, and Misra was a contracted adviser. https://www.nber.org/papers/w23775

**Note 6.**

> Even so, more than 60% of customers would have got lower prices under the personalised scheme; the losses fell on the rest.

Dubé and Misra (NBER w23775): optimising the single (uniform) price raised profit 55%; under personalised pricing, consumer surplus fell about 47% against the status quo (about 23% against the optimised uniform price); "over 60% of consumers benefit from lower prices under personalization". https://www.nber.org/papers/w23775

**Note 7.**

> Among those who didn't seek help for one or more of their problems, 46% gave cost as a reason.

Legal Services Corporation, *Justice Gap* study, 2022 (survey data from 2021), executive summary. https://justicegap.lsc.gov/the-report/executive-summary/

**Note 8.**

> At 100 rupees, about $1.64, enrolment fell by about 17 percentage points, a quarter of the free take-up.

J-PAL evaluation summary of Berry and Mukherjee's tutoring price experiment in Delhi, 2014–16: 5,439 students, 21 low-income neighbourhoods, first prices INR 0–250 (US$0–4.10). https://www.povertyactionlab.org/evaluation/impact-private-tutoring-prices-student-attendance-and-performance-india

**Note 9.**

> And the tutoring had no effect on the children's maths or English scores.

J-PAL evaluation summary (Berry and Mukherjee). https://www.povertyactionlab.org/evaluation/impact-private-tutoring-prices-student-attendance-and-performance-india

**Note 10.**

> Those authors also warn against boiling the experiment down to that single number.

Aron-Dine, Einav and Finkelstein, NBER Working Paper 18642, December 2012, a re-analysis of the RAND Health Insurance Experiment (1974–81). The −0.2 figure is read in their abstract, not in the original RAND reports. https://www.nber.org/papers/w18642

**Note 11.**

> Companies have announced lower prices, and some have announced new hiring, but none that we found publishes both halves with numbers.

Our search of published studies and company statements, October 2026, recorded in the book's research notes (`research_notes/playbook-demand.md`, gap 3; `research_notes/playbook-and-market.md`, 1.4A).

**Note 12.**

> Run it backwards to see what your bar demands: the elasticity you need is =LN(C)/LN(1-D), with D as a fraction.

Our calculation, using the standard constant-elasticity form: volume multiple = (1 − cut) ^ elasticity. At a 25% cut, −0.55 gives 0.75^−0.55 ≈ 1.17; the elasticity needed for 1.67 times is ln(1.67) ÷ ln(0.75) ≈ −1.78. Elasticities from note 3 (Tellis) and note 4 (Uber). The form is a simplification; real demand rarely keeps one elasticity over a large price change.

## Chapter 7: Price Down, Sell Wider

**Note 1.**

> The figures come from a table that Ford's production department compiled in 1927, which survives in later reprints.

Model T production and Runabout list prices by year, compiled by R. E. Houston, Ford Production Department, 3 August 1927, as reproduced in Wikipedia, "Ford Model T" (production table, which cites Lewis, 1976): 1909, 10,666 at $825; 1912, 68,733 at $590; 1916, 501,462 at $345. https://en.wikipedia.org/wiki/Ford_Model_T

**Note 2.**

> Ford's plant at Highland Park was the home of its moving assembly line, which Ford's own history credits with taking output "from hundreds a day to thousands a day."

Ford Motor Company, *From the Road* (2021), article on Highland Park as the birthplace of the moving assembly line. https://www.fromtheroad.ford.com/us/en/articles/2021/highland-park--birthplace-of-moving-assembly-line

**Note 3.**

> In 1912 the plant averaged 6,867 employees; in 1916, 32,702.

The Henry Ford, Benson Ford Research Center, research guide on Ford's average employees by year (from Nevins and Hill): Highland Park series, 6,867 (1912) and 32,702 (1916). Rows before 1910 carry the Highland Park label though the plant opened in 1910. Price fall of 41%, output ×7.3 and payroll ×4.8 (1912 to 1916) are our calculations from these rows and note 1. https://askus.thehenryford.org/researchguides/faq/375645

**Note 4.**

> On that count, Ford employed an average of 48,264 people in 1919 and 155,552 in 1925, more than three times as many.

The Henry Ford, research guide (note 3), US-total series: 48,264 (1919) and 155,552 (1925). The 1919 Runabout price of $500 and the 1925 price of $260 are from the production table in note 1. https://askus.thehenryford.org/researchguides/faq/375645

**Note 5.**

> Then, from 1923 to 1925, the price fell by about 29%, to $260, and production fell by about 5%, to about 1.91 million.

Production table (note 1): 1917, 735,020 at $500; 1922, 1,301,067 at $319; 1923, 2,011,125 at $364; 1925, 1,911,705 at $260. The price rise of 45% and output ×1.47 (1916 to 1917), the price rise of 14% and output ×1.55 (1922 to 1923), and the price fall of 29% and output fall of 5% (1923 to 1925) are our calculations. https://en.wikipedia.org/wiki/Ford_Model_T

**Note 6.**

> The price had gone back up by then, to $360 in 1926, and output fell by about a fifth that year.

Production table (note 1): 1926, 1,554,465 at $360; 1927, 399,725 at $360. The Henry Ford research guide (note 3): 102,029 US employees in 1927. The fall of 34% in employees from 1925 and of 19% in output from 1925 to 1926 are our calculations. Ford's own page gives a Highland Park peak of "almost 70,000" in 1925, a different measure from these payroll averages. https://askus.thehenryford.org/researchguides/faq/375645

**Note 7.**

> Ford's own history says the Model T's price was "reduced from $850 to $260."

Ford Motor Company, *From the Road* (2021), note 2. The fall from $825 to $260 on the Runabout series, about 68%, is our calculation. https://www.fromtheroad.ford.com/us/en/articles/2021/highland-park--birthplace-of-moving-assembly-line

**Note 8.**

> In a November 2011 press release, Andy Jassy said: "Since the launch of AWS over five years ago, we've lowered our prices over a dozen times."

Amazon press release on the new US West (Oregon) region, 9 November 2011. https://press.aboutamazon.com/2011/11/amazon-web-services-announces-new-lower-priced-us-west-region-oregon

**Note 9.**

> "The sales growth primarily reflects increased customer usage, partially offset by pricing changes," the report says, and those changes "were driven largely by our continued efforts to reduce prices for our customers."

Amazon.com, Form 10-K for fiscal 2015: AWS net sales $3,108m (2013), $4,644m (2014), $7,880m (2015). https://www.sec.gov/Archives/edgar/data/0001018724/000101872416000172/amzn-20151231x10k.htm

**Note 10.**

> In 2025 AWS sold about $128.7 billion, about 41 times its 2013 figure.

Amazon.com, fourth-quarter 2025 results, 5 February 2026: AWS segment sales $128,725m in 2025. The 41-fold rise from 2013 is our calculation. https://ir.aboutamazon.com/news-release/news-release-details/2026/Amazon-com-Announces-Fourth-Quarter-Results/default.aspx

**Note 11.**

> Its total workforce was 1,576,000 on 31 December 2025, up 1% on the year before.

Amazon.com, fourth-quarter 2025 results (note 10): 1,576,000 employees at 31 December 2025, up 1%. https://ir.aboutamazon.com/news-release/news-release-details/2026/Amazon-com-Announces-Fourth-Quarter-Results/default.aspx

**Note 12.**

> And Jassy said in June 2025, as reported by SiliconANGLE, that he expects AI to "reduce our total corporate workforce," with "fewer people doing some of the jobs" and "more people doing other types of jobs."

SiliconANGLE, 17 June 2025. https://siliconangle.com/2025/06/17/andy-jassy-says-generative-ai-will-reduce-amazons-workforce-coming-years/

**Note 13.**

> Paul Philip, the regulator's chief executive, called it "a landmark moment for legal services in this country."

Solicitors Regulation Authority, news release on the authorisation of Garfield.Law, 6 May 2025. https://www.sra.org.uk/sra/news/press/garfield-ai-authorised/

**Note 14.**

> Its prices start at £2 for what it calls a "polite chaser" letter, the legal news site Legal Cheek reported, and it handles claims of up to £10,000, mostly for small firms chasing debts.

Legal Cheek, 6 May 2025. https://www.legalcheek.com/2025/05/sra-approves-ai-driven-law-firm/

**Note 15.**

> In May 2024 Khan Academy made Khanmigo for Teachers, its AI assistant, free for every teacher in the United States, thanks to Microsoft, which "donated access to infrastructure."

Khan Academy blog, 20 May 2024 (updated 20 March 2025), headed "Thanks to Microsoft Support". https://blog.khanacademy.org/?p=16370

**Note 16.**

> In May 2024 Khan Academy made Khanmigo for Teachers, its AI assistant, free for every teacher in the United States, thanks to Microsoft, which "donated access to infrastructure." At the time, CNBC reported, about 65,000 students and teachers were using Khanmigo in their classes, school districts paid about $35 per student a year, and Khan hoped the cost could later come down to $10 to $20.

CNBC (Eric Rosenbaum), via NBC New York, 21 May 2024. The 65,000 users and the $35 price refer to the Khanmigo tutoring tool that school districts pay for, a different product from the free teacher assistant. https://www.nbcnewyork.com/news/business/money-report/microsoft-launches-free-ai-assistant-for-all-educators-in-us-in-deal-with-khan-academy/5433259/

**Note 17.**

> By Zerodha's account, its chief executive, C Vijayakumar, had said a quarter earlier that each dollar of revenue now took his teams roughly 25% to 30% more effort than before.

Zerodha, *The Daily Brief*, article dated 28 July 2026. Vijayakumar's figure is Zerodha's account of a remark made the previous quarter. https://thedailybrief.zerodha.com/p/it-results-ai-impact-indigo-loss-fuel-costs-weak-rupee

**Note 18.**

> Wipro grew 4%.

*The Register*, 28 April 2026, on the fiscal 2026 results of TCS, Infosys, Wipro and HCLTech. https://www.theregister.com/2026/04/28/tcs_infosys_wipro_hcl_fy26/

**Note 19.**

> Krithivasan himself had said that month that clients were slow to decide and to start projects, and the report quotes nothing from him linking the cuts to AI.

Reuters, via Yahoo Finance, 27 July 2025. Reuters gives the cut as "roughly 12,200" jobs. https://finance.yahoo.com/news/indian-tech-company-tcs-cut-103558769.html

**Note 20.**

> A year later the Zerodha report put TCS at about 5.94 lakh employees, roughly 594,000, with a small net gain that quarter, while HCLTech's headcount fell by about 3,300 in the same quarter.

Zerodha, *The Daily Brief* (note 17). A lakh is 100,000. https://thedailybrief.zerodha.com/p/it-results-ai-impact-indigo-loss-fuel-costs-weak-rupee

**Note 21.**

> Added up from the firms' own reports, the combined staff of the four largest Indian IT firms (TCS, Infosys, Wipro and HCLTech) peaked in March 2023, and by June 2026 it was 3.6% below that peak.

Firms' own reported total headcounts, summed by us; every figure, page and saved copy is in
`analysis/data/part3/t1_t6/it_headcounts.csv` (sources in `analysis/data/part3/t1_t6/SOURCES.md`), retrieved
2026-10-22. March 2023: TCS 614,795, Infosys 343,234, Wipro 256,921, HCLTech 225,944; total 1,440,894. June 2026:
TCS 593,798, Infosys 328,062, Wipro 243,044, HCLTech 223,889; total 1,388,793, which is 3.6% below March 2023.
Sources: TCS, Q4 FY2022-23 Fact Sheet, p. 18,
https://web.archive.org/web/20230511130443id_/https://www.tcs.com/content/dam/tcs/investor-relations/financial-statements/2022-23/q4/Presentations/Q4%20FY%202022-23%20Fact%20sheet.pdf ,
and Q1 2026-27 Fact Sheet, p. 12,
https://web.archive.org/web/20260828130818id_/https://www.tcs.com/content/dam/tcs/investor-relations/financial-statements/2026-27/q1/Presentations/Q1%202026-27%20Fact%20Sheet.pdf ;
Infosys, Q4 2022-23 fact sheet, p. 2,
https://web.archive.org/web/20251128200537id_/https://www.infosys.com/investors/reports-filings/quarterly-results/2022-2023/q4/documents/fact-sheet.pdf ,
and Q1 2026-27 fact sheet, p. 2,
https://web.archive.org/web/20260828130817id_/https://www.infosys.com/investors/reports-filings/quarterly-results/2026-2027/q1/documents/fact-sheet.pdf ;
Wipro, Q4 FY23 datasheet, p. 4,
https://www.wipro.com/content/dam/nexus/en/investor/quarterly-results/2022-2023/q4fy23/datasheet-q4fy23.pdf , and
Q1 FY27 datasheet, p. 3,
https://www.wipro.com/content/dam/nexus/en/investor/quarterly-results/2026-2027/q1fy27/datasheet-q1fy27.pdf ;
HCLTech, Q4 FY24 Investor Release, p. 20,
https://www.hcltech.com/sites/default/files/documents/investor-reports/HCLTech_Q4_FY24_Investor_Release.pdf , and
Q1 FY27 Investor Release, p. 9,
https://www.hcltech.com/sites/default/files/documents/investor-reports/HCLTech_Q1_FY27_Investor_Release.pdf .
Wipro counts are as first reported: March 2023 was later restated to 258,570 to include the ISRE business. HCLTech's
FY25 figure includes a 7,398 reduction from a divestiture, and HCLTech reached a new high (230,339) in September
2026. June 2026 is the latest date with all four firms (Infosys's September 2026 figure was not found). The four
firms grew 49.8% from March 2019 to the 2023 peak, a hiring burst that predates ChatGPT.

**Note 22.**

> In the United States, jobs in computer systems design were 10.7% below their 2015-19 trend in the year to September 2026, and have fallen about 5% since December 2022.

Our calculation, descriptive series T6, code in `analysis/part3/t1_t6/`, results in
`analysis/results_part3_t1_t6.json`, red-team checks in `analysis/part3/redteam/rt_t1_t6.py` (REDTEAM.md, T6).
Data: BLS, Current Employment Statistics, series CES6054150001, all employees, computer systems design and related
services (NAICS 5415), seasonally adjusted,
https://data.bls.gov/timeseries/CES6054150001?from_year=2010&to_year=2026&output_view=data&include_graphs=false ,
retrieved 2026-10-22 (August and September 2026 preliminary; the March 2026 benchmark revision is not yet in them).
Average employment October 2025 to September 2026 was 2,370.8 thousand against 2,654.2 thousand on a straight line
fitted to 2015-2019, a gap of -10.7% (95% bootstrap interval -11.6 to -9.7, covering only the trend line's
uncertainty). Employment fell 5.1% from December 2022. In pre-AI history, 15 of 19 straight-line trends extended
the same distance missed by at least 10.7 points, so the gap is not on its own evidence about AI; the whole
information sector is also 11.4% below its trend. The gap coincides with higher interest rates (2022-23) and the end
of pandemic over-hiring.

**Note 23.**

> "We believe the pie will increase." He expects AI to raise output by 20% to 30% in conventional IT work, with the gains going to work clients have long put off.

People Matters, 19 February 2026, relaying CNBC-TV18. The 20% to 30% figure is a paraphrase in that report. https://www.peoplematters.in/news/leadership/ai-productivity-gains-wont-lead-to-headcount-cuts-says-tcs-ceo-48488

## Chapter 8: Build What Wasn't Worth Building

**Note 1.**

> Most of the trade the authors looked at ran from American sellers to buyers in Spanish-speaking Latin America.

Brynjolfsson, Hui and Liu, "Does Machine Translation Affect International Trade? Evidence from a Large Digital Platform", *Management Science* 65(12), 2019 (published abstract, MIT DSpace: exports up 10.9%; the abstract says "a digital platform", and eBay is named in the working paper), https://dspace.mit.edu/handle/1721.1/129711 ; NBER Working Paper 24917, August 2018, working-paper version, which put the rise at 17.5%; its non-technical summary describes it in terms of US exports to Spanish-speaking Latin American countries. https://www.nber.org/papers/w24917

**Note 2.**

> The authors draw a plain conclusion: language barriers had been holding trade back, and AI had begun to improve economic efficiency "in at least one domain."

Brynjolfsson, Hui and Liu (2019), abstract. https://dspace.mit.edu/handle/1721.1/129711

**Note 3.**

> By 2006 the cost of a draft was down to about $14 million, by the middle of 2015 to just above $4,000, and by late 2015 to below $1,500.

National Human Genome Research Institute, "The Cost of Sequencing a Human Genome", fact sheet, last updated 1 November 2021 (draft produced April 1999 to June 2000). The fall of more than 200,000 times is our calculation from the draft figures ($300 million to under $1,500); the first reference genome ($500 million to $1 billion) is a different measure and is left out of it. https://www.genome.gov/about-genomics/fact-sheets/Sequencing-Human-Genome-cost

**Note 4.**

> Using résumés to gauge how much firms put into AI, the authors found that the heavier investors, on average, added sales and staff faster than the rest.

T. Babina, A. Fedyk, A. He and J. Hodson, "Artificial intelligence, firm growth, and product innovation", *Journal of Financial Economics* 151 (2024), 103745, abstract. https://ideas.repec.org/a/eee/jfinec/v151y2024ics0304405x2300185x.html

**Note 5.**

> Patents on processes, the ways a firm makes what it already sells, rose by "just over 1%," a result that was not statistically significant.

T. Babina and A. Fedyk, "The effects of AI on firms and workers", Brookings, 1 July 2025 (the authors' summary of their research; the journal's tables were not read for this book): trademarks and patents, 2010 to 2018. https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/

**Note 6.**

> The authors' own summary is that the growth "comes primarily through increased product innovation." They add that AI "has so far not led to widespread job loss," and that its main use so far doesn't appear to be cutting costs and replacing workers.

Babina, Fedyk, He and Hodson (2024), abstract ("This growth comes primarily through increased product innovation"), https://ideas.repec.org/a/eee/jfinec/v151y2024ics0304405x2300185x.html ; Babina and Fedyk, Brookings (2025), https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/

**Note 7.**

> First, the sales took time: they followed about two to three years after the investment began.

Babina and Fedyk, Brookings (2025): "approximately two to three years". https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/

**Note 8.**

> The authors write that larger firms, with more data and more money to spend, "can reap greater benefits," and the journal paper finds that AI-powered growth "concentrates among larger firms and is associated with higher industry concentration."

Babina and Fedyk, Brookings (2025), https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/ ; Babina, Fedyk, He and Hodson (2024), abstract. https://ideas.repec.org/a/eee/jfinec/v151y2024ics0304405x2300185x.html

**Note 9.**

> The share of junior employees rose by 1.6%, while the shares of middle managers and senior managers fell by 0.8% and 0.7%.

Babina and Fedyk, Brookings (2025): all four figures are changes in shares of the workforce. https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/

**Note 10.**

> In December 2025, by its count, more than 6 million viewers a day watched at least ten minutes of dubbed content.

YouTube Official Blog, on auto dubbing and Expressive Speech, 4 February 2026: "more than 6 million daily viewers who watched at least 10 minutes of auto dubbed content" in December. https://blog.youtube/news-and-events/youtube-auto-dubbing-expressive-speech/

**Note 11.**

> Its chief executive, Luis von Ahn, said the first 100 had taken about 12 years, and these nearly 150 took about a year (as reported by FOX 29).

FOX 29, 1 May 2025, reporting Duolingo's announcement and quoting von Ahn: "Developing our first 100 courses took about 12 years, and now, in about a year, we're able to create and launch nearly 150 new courses." Duolingo's own release could not be reached. https://www.fox29.com/news/duolingo-148-courses-ai

**Note 12.**

> Von Ahn said the firm had never laid off full-time employees and didn't plan to, and that "one person will be able to accomplish more." An earlier memo had set out a gradual reduction in contractors, and he said the contractor force "has gone up and down depending on needs," as reported by *Fortune*, relaying the *New York Times*.

*Fortune*, 18 August 2025, relaying the *New York Times*. Neither this report nor HCAMag (10 October 2025), which says only that Duolingo announced in April it would "gradually stop using contractors to do work that AI can handle", gives numbers or says how far the plan went. https://fortune.com/2025/08/18/duolingo-ceo-admits-controversial-ai-memo-did-not-give-enough-context-insists-company-never-laid-off-full-time-employees

**Note 13.**

> The students gained about 0.31 standard deviations overall and 0.23 in English, the main measure.

De Simone, Tiberti, Barron Rodriguez, Manolio, Mosuro and Dikoru, World Bank Policy Research Working Paper 11125 (2025), working-paper version, abstract. https://reproducibility.worldbank.org/catalog/419

**Note 14.**

> The authors put that at 1.5 to 2 years of ordinary schooling, and the Bank's education team wrote that it outperformed 80% of the programmes in its database of trials in developing countries.

De Simone et al. (2025), abstract ("1.5 to 2 years of 'business-as-usual' schooling"); World Bank Education blog, "From chalkboards to chatbots", 9 January 2025 ("our program outperformed 80% of them"). https://blogs.worldbank.org/en/education/From-chalkboards-to-chatbots-Transforming-learning-in-Nigeria

**Note 15.**

> Among the 194 students analysed, the median learning gain with the AI tutor was more than twice as large, and the students took a median of 49 minutes, against a 60-minute class.

Kestin, Miller et al., *Scientific Reports* 15:17458, 3 June 2025: 194 students analysed of 233 enrolled; regression effect 0.63 standard deviations; two lessons in consecutive weeks of one introductory physics course, autumn 2023. https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/

**Note 16.**

> Base44 had about 250,000 users and made about $189,000 in profit in May 2025.

TechCrunch, 18 June 2025 (Wix's own release was not reached). https://techcrunch.com/2025/06/18/6-month-old-solo-owned-vibe-coder-base44-sells-to-wix-for-80m-cash

**Note 17.**

> About 1.1 million public projects on the site now use a toolkit for building on a large language model.

GitHub, *Octoverse 2025*, GitHub blog, 28 October 2025 (updated 28 February 2026), covering September 2024 to August 2025: "Roughly 80% of new GitHub users tried Copilot within their first week." https://github.blog/news-insights/octoverse/octoverse-a-new-developer-joins-github-every-second-as-ai-leads-typescript-to-1/

**Note 18.**

> Some 85% of users said they spent time saved on other tasks, and fewer than 10% said they took more breaks.

A. Humlum and E. Vestergaard, "Still Waters, Rapid Currents", NBER Working Paper 33777 (May 2025, revised March 2026), working-paper version. The share with new tasks under employer initiatives is "roughly 18%" in the body (p. 14) and "roughly 17%" in the introduction. https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 19.**

> Even people who didn't use the tools picked up new work: 4% of non-users reported new AI workloads, and 10% of teachers who didn't use AI themselves reported new work checking their students' use of it.

Humlum and Vestergaard (revised March 2026). The paper groups six task categories into these three (42% is three of them, 35% two, 26% one). The three add to about 103% as printed, and the paper does not explain the difference. https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 20.**

> The same study, as chapter 1 noted, could rule out any effect on earnings or hours above 2%, two years on from ChatGPT's launch.

Humlum and Vestergaard (revised March 2026). https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 21.**

> Forward-deployed engineers and product managers were only about 9,000, but their numbers had grown 42-fold since 2023.

LinkedIn Economic Graph, *Labor Market Report: Building a Future of Work That Works*, January 2026, p. 10 (chart values read from the figure; report read via a mirror). https://www.bollettinoadapt.it/wp-content/uploads/2026/01/linkedIn-labor-market-report-building-a-future-of-work-that-works-jan-2026.pdf

**Note 22.**

> In marketing the share rose during 2025 from 8.4% to 14.9%, and in human resources from 4.4% to 8.8%.

Cory Stahle, Indeed Hiring Lab, January 2026 labor market update, 22 January 2026. https://hiringlab.indeed.com/2026/01/22/january-labor-market-update-jobs-mentioning-ai-are-growing-amid-broader-hiring-weakness/

## Chapter 9: Augment Before You Automate

**Note 1.**

> The researchers split them into three groups: one worked without AI, one was given GPT-4, and one was given GPT-4 along with a short overview of how to prompt it.

Dell'Acqua, McFowland, Mollick, Lifshitz-Assaf, Kellogg, Rajendran, Krayer, Candelon and Lakhani, "Navigating the Jagged Technological Frontier: Field Experimental Evidence of the Effects of AI on Knowledge Worker Productivity and Quality", Harvard Business School Working Paper 24-013, 22 September 2023 (SSRN 4573321), abstract: sample, pre-registration and the three groups. https://mitsloan.mit.edu/sites/default/files/2023-10/SSRN-id4573321.pdf

**Note 2.**

> In the paper's headline figure, their work scored more than 40% higher on quality than the group without AI.

Dell'Acqua et al. (2023), abstract: 18 tasks, 12.2%, 25.1% and "more than 40% higher quality compared to a control group".

**Note 3.**

> In the group with the prompting overview, they spent more than 11 minutes less, a cut of 30%.

Dell'Acqua et al. (2023), section on the task outside the frontier and Table 4: 84.5% for the control group against about 60% and 70%, down 24 percentage points (GPT-4 with overview) and 13 (GPT-4 only); the difference between the two AI groups is significant only at the 10% level. Time: Table 5 discussion.

**Note 4.**

> Those below the average performance threshold improved by 43% and those above it by 17%, each measured against their own scores.

Dell'Acqua et al. (2023), abstract.

**Note 5.**

> The authors warn that while AI helps produce better content, it "might lead to more homogenized outputs," with less variety in the ideas.

Dell'Acqua et al. (2023), results and Appendix D.

**Note 6.**

> The group given the prompting overview kept more of GPT-4's text unchanged than the group given GPT-4 alone.

Dell'Acqua et al. (2023), Appendix C.

**Note 7.**

> A version was published in *Organization Science* in March 2026, and its abstract keeps the 12.2% and 25.1% gains and "significantly improved quality," but drops the 40% quality figure and the 43% and 17% split.

The same nine authors, *Organization Science* 37(2): 403-423, March 2026, DOI 10.1287/orsc.2025.21838; abstract and metadata via Crossref. The journal's full text could not be read. https://api.crossref.org/works/10.1287/orsc.2025.21838

**Note 8.**

> And the study is partly BCG's own: three of the nine authors work for the firm, and one more, Lakhani, advises it on AI strategy.

Dell'Acqua et al. (2023), title page.

**Note 9.**

> These consultants kept a "strategic division of labor between humans and machines," and switched between AI and their own work, "allocating responsibilities based on the strengths and capabilities of each entity." Others they called "cyborgs," who "intertwine their efforts with AI at the very frontier of capabilities," handing work back and forth within a single task, starting a sentence, say, for the AI to finish.

Dell'Acqua et al. (2023), section on patterns of use: the strategies of consultants who answered the outside-the-frontier task correctly while using AI.

**Note 10.**

> The trial covered 640 business owners and was published in *Management Science* in July 2026.

Otis et al., randomised trial with 640 Kenyan entrepreneurs, *Management Science*, published online 10 July 2026, DOI 10.1287/mnsc.2024.06909. https://api.crossref.org/works/10.1287/mnsc.2024.06909 ; author copy: https://escholarship.org/content/qt0fb001r8/qt0fb001r8.pdf

**Note 11.**

> In the authors' subsample analyses, low performers "did nearly 10% worse because of the AI assistant," while high performers "may have benefited by over 15%." The difference lay in the advice each group chose to act on.

Otis et al. (2026), abstract and author copy (note 10).

**Note 12.**

> After, the figure was 22.4% (145 of 648).

Budzyń et al., *Lancet Gastroenterology & Hepatology* 2025;10(10):896-903, abstract (PubMed 40816301). Observational study in four Polish centres; an erratum and letters have been published. https://pubmed.ncbi.nlm.nih.gov/40816301/

**Note 13.**

> Their examples of so-so technology include "several of the applications of artificial intelligence technology to tasks that are currently challenging for machines."

D. Acemoglu and P. Restrepo, "Automation and New Tasks: How Technology Displaces and Reinstates Labor", *Journal of Economic Perspectives* 33(2): 3-30, 2019; version read: NBER Working Paper 25684, March 2019. https://www.nber.org/system/files/working_papers/w25684/w25684.pdf

**Note 14.**

> In 30%, jobs connected with building and running the AI were growing.

Milanez, "The impact of AI on the workplace: Evidence from OECD case studies of AI implementation", OECD Social, Employment and Migration Working Papers No. 289, 2023. https://www.oecd.org/content/dam/oecd/en/publications/reports/2023/03/the-impact-of-ai-on-the-workplace-evidence-from-oecd-case-studies-of-ai-implementation_b4c2c6ee/2247ce58-en.pdf

**Note 15.**

> When AI automated a task it could do more quickly or cheaply, Milanez writes, "demand for human workers to do the other tasks around the AI rose."

Milanez (2023), note 14.

**Note 16.**

> And the paper cautions that the cases may carry "a positive skew" in the AI uses selected.

Milanez (2023), note 14: "a positive skew to the AI use cases selected".

**Note 17.**

> Where employers encouraged use and also provided company chatbots and training, 93% of workers had used AI chatbots at work, 28% used them daily, and 19% said they saved more than an hour a day.

Humlum and Vestergaard, "Still Waters, Rapid Currents", NBER Working Paper 33777 (revised March 2026), introduction: 93%, 28% and 19% for workplaces combining "encouraged use with enterprise chatbots and training". The new-tasks finding is in chapter 8. https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

**Note 18.**

> In a 2024 paper he argues that "the unique opportunity that AI offers to the labor market is to extend the relevance, reach, and value of human expertise," letting "a larger set of workers possessing complementary knowledge" take on decisions now kept for elite experts.

Autor, "Applying AI to Rebuild Middle Class Jobs", NBER Working Paper 32140, February 2024. https://www.nber.org/system/files/working_papers/w32140/w32140.pdf

**Note 19.**

> He is careful about what this proves: "There is no economic law that says that the forces of automation and new work creation are equal and offsetting," and his thesis "is not a forecast but an argument about what is possible."

Autor (2024), note 18.

**Note 20.**

> One adviser quoted in the firm's release said it was "saving me about half an hour per meeting." The firm's line on what stays human was that the human touch "remains fundamental."

Morgan Stanley, press release on the launch of AI @ Morgan Stanley Debrief, 26 June 2024. The assistant launched in September 2023. https://www.morganstanley.com/press-releases/ai-at-morgan-stanley-debrief-launch

**Note 21.**

> One adviser quoted in the firm's release said it was "saving me about half an hour per meeting." The firm's line on what stays human was that the human touch "remains fundamental." OpenAI reported on its own customer page that access to the firm's documents "jumped from 20% to 80%."

OpenAI, customer story on Morgan Stanley, undated, as archived on 14 October 2026. https://web.archive.org/web/20261014180350/https://openai.com/index/morgan-stanley/

**Note 22.**

> The bank says this has been "significantly decreasing call center volume and allowing financial specialists to spend time focusing on more complex financial conversations." An internal version is used by over 90% of staff and has "reduced calls into the IT service desk by 50%."

Bank of America, press release, 20 August 2025. https://newsroom.bankofamerica.com/content/newsroom/press-releases/2025/08/a-decade-of-ai-innovation--bofa-s-virtual-assistant-erica-surpas.html

**Note 23.**

> The figure that matters most here is another one: customers needed 20% less follow-up contact.

Telstra, media release "Telstra scales up AI adoption", 7 February 2024. https://www.telstra.com.au/aboutus/media/media-releases/telstra-scales-up-ai-adoption

**Note 24.**

> They say nothing for or against the firm-level design advice in this chapter.

Our calculation, pre-registered test T4 (augmentation split), code in `analysis/part3/t4_t5/`, results in
`analysis/results_part3_t4_t5.json`, red-team checks in `analysis/part3/redteam/rt_t4_t5.py` and `rt_extra.py`
(REDTEAM.md, T4 augmentation). Employment data as in note p3b (BLS OEWS, May 2016-2025). Augmentation share: Anthropic
Economic Index, release 2025-03-27 (the README's citation for this release: Handa, K. et al., "Which Economic Tasks
are Performed with AI? Evidence from Millions of Claude Conversations", arXiv:2503.04761, 2025),
https://huggingface.co/datasets/Anthropic/EconomicIndex, CC BY; modified (aggregated to occupations). Tasks were
moved to occupations with O*NET data: "This includes information from the O*NET 31.0 Database by the U.S. Department
of Labor, Employment and Training Administration (USDOL/ETA). Used under the CC BY 4.0 license. O*NET® is a trademark
of USDOL/ETA. The author has modified all or some of this information. USDOL/ETA has not approved, endorsed, or tested these
modifications." (wording as recorded in `analysis/data/part3/t4_t5/SOURCES.md`; licence at
https://www.onetcenter.org/license_db.html; crosswalk
https://www.onetcenter.org/taxonomy/2019/walk/2010_to_2019_Crosswalk.csv). Within the two most exposed
fifths (282 occupation units with usage data), the more augmentative half grew -1.05 points a year relative to the
more automated half, 2022-2025 (95% interval -2.60 to +0.68), against -0.91 in 2016-2019; main minus placebo -0.14
(interval -2.20 to +1.84). Caveats: the measure comes from one company's chatbot conversations in early 2025, after
most of the outcome window; usage per occupation is thin; it describes how people phrase requests, not how employers
deploy AI. The test asks about occupations, not firms, and neither supports nor contradicts chapter 9's firm-level
advice.

## Chapter 10: Redeploy and Retrain

**Note 1.**

> Asked whether the bot meant job cuts, the company answered: "That's not what we're seeing right now."

Reuters (Helen Reid), "IKEA bets on remote interior design as AI changes sales strategy", 13 June 2023, as carried by *The Globe and Mail*. Ingka's own figures as reported by Reuters; no Ingka statement confirming the 8,500 or the 47% was found. https://theglobeandmail.com/business/international-business/article-ikea-bets-on-remote-interior-design-as-ai-changes-sales-strategy/

**Note 2.**

> What Ingka has published is a plan, from April 2024, to train about 30,000 of its staff and 500 of its leaders in the basics of AI.

Ingka Group newsroom, "IKEA Retail unleashes AI revolution, empowering thousands to master the future of tech", 12 April 2024: "approximately 30,000 co-workers and 500 leaders" from financial year 2024. https://www.ingka.com/newsroom/ikea-retail-unleashes-ai-revolution-empowering-thousands-to-master-the-future-of-tech/

**Note 3.**

> IBM says the tool settles 94% of them without a person and handled more than 11.5 million conversations with employees in 2024, and that the HR team's operating costs fell by 40% over four years.

IBM, "IBM AskHR" case study (company page): "94% containment rate of common questions", "more than 11.5 million employee interactions in 2024", "40% reduction in the HR team's operational costs over the past four years". No headcount or redeployment figures given. https://www.ibm.com/case-studies/ibm-askhr

**Note 4.**

> He also said: "Our total employment has actually gone up." A later report relaying the newspaper said IBM's hiring grew in programming, sales, marketing and software engineering.

SHRM, 12 May 2025, reporting Krishna's interview with the *Wall Street Journal*. https://www.shrm.org/in/topics-tools/flagships/ai-hi/ibm-embraces-ai--reduces-hr-roles ; on the areas where hiring grew, HR Reporter, 24 July 2025, relaying the *Wall Street Journal*. https://www.hrreporter.com/focus-areas/automation-ai/with-ibm-laying-off-100s-of-hr-people-is-automation-replacing-hr/393063

**Note 5.**

> Their finding, first published in 2020, was that the programmes "generate substantial and persistent earnings gains (11 to 40 percent) following training completion."

L. F. Katz, J. Roth, R. Hendra and K. Schaberg, "Why Do Sectoral Employment Programs Work? Lessons from WorkAdvance", NBER Working Paper 28248, December 2020, abstract; published in *Journal of Labor Economics* 40(S1), 2022, S249-S291. https://www.nber.org/papers/w28248

**Note 6.**

> In the same evaluators' series the gain had been 38% at about three years; the share fell because the comparison group's earnings had risen, and the evaluators wrote that the gains "persisted undiminished." They put the net benefit to society at $33,884 per participant, or $2.46 back for each dollar spent.

Fein and Dastrup, Abt Associates, PACE long-term impact report on Year Up, OPRE Report 2022-77, 2022 (seven years: quarters 23-24; the earlier 38% is for quarters 12-13; the cost-benefit figures are for the seven-year period). https://www.abtglobal.com/files/insights/reports/2022/year%20up%20long-term%20impact%20report_apr2022.pdf

**Note 7.**

> Many participants worked fewer hours, or none, while they were at college, so for the first year or two they earned less than the comparison group.

Economic Mobility Corporation, Project QUEST 14-year results, October 2024 (410 participants; cost in 2022 dollars). https://economicmobilitycorp.org/wp-content/uploads/2024/10/Project-Quest-14-Year-Gains.pdf

**Note 8.**

> At the other three sites there were "no statistically significant effects on average earnings." Their own conclusion: "not all sector programs will lead to increases in employment and earnings."

MDRC (Kanengiser and Schaberg), "Employment and Earnings Effects of the WorkAdvance Demonstration After Seven Years", March 2022. https://www.mdrc.org/work/publications/employment-and-earnings-effects-workadvance-demonstration-after-seven-years

**Note 9.**

> Average effects were "close to zero in the short run," and became "more positive 2-3 years after completion." Programmes that put the weight on building skills showed larger average gains.

D. Card, J. Kluve and A. Weber, "What Works? A Meta Analysis of Recent Active Labor Market Program Evaluations", NBER Working Paper 21431 (2015, revised 2017), abstract; published in *Journal of the European Economic Association* 16(3), 2018, 894-931. https://www.nber.org/papers/w21431

**Note 10.**

> In a summary of this research, the WorkRise network describes what these programmes typically do: careful screening of applicants, training for a specific sector along with workplace skills, help with problems outside the classroom, placement into jobs and, in many of them, close ties to employers.

WorkRise, *Working Knowledge* summary of the sector-focused training evidence in NBER w28248 (December 2020). https://www.workrisenetwork.org/working-knowledge/evidence-sector-focused-training-programs-shows-significant-and-persistent

**Note 11.**

> It says apprentices in its mechatronics and robotics programme see a wage rise of nearly 23% after classroom training and a further 26% after training on the job.

Amazon, "Amazon employees upskilling, education and training" (company page, undated, read in its 2025 form). Self-reported, with no comparison group. https://aboutamazon.com/news/workplace/amazon-employees-upskilling-education-training

**Note 12.**

> Fortune reported in 2017 that the company was retraining more than 100,000 workers in a "roughly billion-dollar push" and had given more than 40% of its open jobs to people already on staff.

*Fortune*, World's Greatest Leaders 2017, entry on Randall Stephenson. https://fortune.com/ranking/worlds-greatest-leaders/2017/randall-stephenson

**Note 13.**

> In 2019 its head of HR told *Chief Learning Officer* that AT&T spent "about $200 million a year" on internal training, and the magazine reported her as saying that staff who had trained were 50% more likely to get a new job inside the company.

*Chief Learning Officer*, "A fixed gaze toward the future", 18 June 2019, interview with AT&T's senior vice president of HR. https://www.chieflearningofficer.com/2019/06/18/a-fixed-gaze-toward-the-future/

**Note 14.**

> Citing a study by the Lumina Foundation, it says participants leave the company at a rate four times lower and are twice as likely to be promoted.

Walmart, Live Better U fact sheet, 17 August 2023, citing a Lumina Foundation study (September 2021). https://corporate.walmart.com/content/dam/corporate/documents/about/working-at-walmart/live-better-u.pdf

**Note 15.**

> Its results release described two paths: "investing in upskilling people, which is its primary focus; exiting people in a compressed timeline where reskilling is not a viable path for the skills it needs." In the same release, it said it expected to increase its total number of employees in the coming financial year.

> It came from the press's own arithmetic: Accenture's total headcount fell from about 791,000 at the end of May to about 779,000 at the end of August, a net change after both leavers and new hires.

Accenture, fourth-quarter and full-year fiscal 2025 results, 25 September 2025: business-optimisation costs of $615 million in the fourth quarter ("$344 million for employee severance and $271 million" for other items) and about $250 million expected in the first quarter of fiscal 2026, about $865 million in all; "approximately 779,000 people". https://newsroom.accenture.com/content/4q-full-fy25-earnings/accenture-reports-fourth-quarter-and-full-year-fiscal-2025-results.pdf ; for the end of May, Accenture, third-quarter fiscal 2025 results, 20 June 2025: "approximately 791,000 people". https://newsroom.accenture.com/content/3qfy25-earnings/accenture-reports-third-quarter-fiscal-2025-results.pdf

**Note 16.**

> On the results call, as *The Register* reported, the chief executive, Sweet, said Accenture had 77,000 "trained AI professionals" on staff, up from 40,000 in 2023.

*The Register*, 26 September 2025, reporting Sweet's remarks on the results call (the 77,000 and 40,000). https://www.theregister.com/2025/09/26/accenture_ai_jobs/

**Note 17.**

> On 27 February 2024, Klarna announced that its AI assistant had handled 2.3 million conversations in its first month, "two-thirds of Klarna's customer service chats." It said the assistant was doing "the equivalent work of 700 full-time agents," had brought the time to settle a customer's problem down from 11 minutes to under 2, and would add an estimated "$40 million USD in profit improvement" in 2024.

Klarna press release, 27 February 2024. https://www.klarna.com/international/press/klarna-ai-assistant-handles-two-thirds-of-customer-service-chats-in-its-first-month/

**Note 18.**

> The AI assistant came almost two years later.

Euronews, 24 May 2022. https://www.euronews.com/2022/05/24/swedish-buy-now-pay-later-firm-klarna-to-lay-off-10-of-staff-citing-likely-recession

**Note 19.**

> CNBC reported, from the filing for Klarna's American share listing, that its full-time staff fell from 5,527 in December 2022 to 3,422 in December 2024, with natural attrition running at 15% to 20% a year.

CNBC, 14 May 2025, as carried by NBC New York, citing Klarna's F-1 filing. The filing itself was not read. https://www.nbcnewyork.com/news/business/money-report/klarna-ceo-says-ai-helped-company-shrink-workforce-by-40/6264593/

**Note 20.**

> Klarna's own release for the first quarter of 2025, in May, said the workforce was about 40% smaller than in 2022, and that customer-service costs per transaction had fallen by 40% since early 2023 "whilst maintaining customer satisfaction levels."

Klarna press release on first-quarter 2025 results, 19 May 2025. https://www.klarna.com/international/press/klarna-accelerates-global-momentum-in-q1-2025-and-unlocks-large-gains-from/

**Note 21.**

> It quoted him directly too: "Really, investing in the quality of human support is the way of the future for us." CNBC reported that Klarna would recruit human agents again, "in an Uber type of setup."

*Entrepreneur*, 9 May 2025, relaying Siemiatkowski's interview with Bloomberg ("wasn't the right path" is the reporter's paraphrase; the second passage is a direct quote). https://www.entrepreneur.com/business-news/klarna-ceo-reverses-course-by-hiring-more-humans-not-ai/491396 ; and CNBC, 14 May 2025 (note 19), for "in an Uber type of setup".

**Note 22.**

> In results published on 19 February 2026, Klarna said headcount was down 49% since 2022 and revenue per employee was up 3.6 times.

Klarna press release on full-year 2025 results, 19 February 2026: "Revenue per employee reached $1.24 million, up 3.6 times since 2022 as headcount declined 49%." https://www.klarna.com/international/press/klarna-accelerates-u-s-growth-and-delivers-usd1bn-revenue-driven-by-rapid/

**Note 23.**

> The research firm Forrester has forecast that half of the layoffs blamed on AI will be "quietly reversed, with jobs returning offshore or at lower wages."

Forrester, "Future of Work Predictions 2026", 12 November 2025 (a forecast). http://www.forrester.com/blogs/future-of-work-predictions-2026-whats-coming-for-work-and-the-workforce/

**Note 24.**

> In July, the Finance Sector Union said a total of 90 jobs were due to be cut: 45 Direct Banking roles because of the bot, plus roles in customer messaging, with some of that work, the union alleged, moving to CBA's operation in India.

Finance Sector Union, 29 July 2025 (the union's account). https://www.fsunion.org.au/?p=6761

**Note 25.**

> The union disputed it.

People Matters (ANZ), 21 August 2025, on CBA's reversal. https://anz.peoplemattersglobal.com/news/hr-technology/commonwealth-bank-of-australia-reverses-plan-to-cut-45-customer-service-roles-after-union-challenge-46533

**Note 26.**

> According to Information Age, the union said call volumes were in fact rising, with staff working overtime and team leaders taking calls themselves.

Information Age (ACS), 21 August 2025. https://ia.acs.org.au/article/2025/cba-reverses-ai-driven-job-cuts--admits--error-.html

**Note 27.**

> The union reported that management "admitted they didn't properly consider that an increase in calls would continue over a number of months," and that CBA would apologise to the 45 staff.

Finance Sector Union, "Win: CBA backflips on customer service job cuts, admits they got it wrong", 21 August 2025 (the union's account). https://www.fsunion.org.au/win-cba-backflips-on-customer-service-job-cuts-admits-they-got-it-wrong/

**Note 28.**

> Information Age reported the bank as saying its assessment "did not adequately consider all relevant business considerations." The 45 could stay, move to other roles, or take redundancy.

Information Age (ACS), 21 August 2025. No CBA newsroom statement was found. https://ia.acs.org.au/article/2025/cba-reverses-ai-driven-job-cuts--admits--error-.html

**Note 29.**

> As HR Review reported it, 39% had made people redundant after bringing in AI, and 55% of those said they had got those decisions wrong.

HR Review, 29 April 2025, reporting Orgvue's survey of about 1,000 senior leaders; the Orgvue report itself could not be reached. https://hrreview.co.uk/hr-news/strategy-news/ai-regret-redundancies-got-them-wrong/381820

## Chapter 11: Keep the Ladder

**Note 1.**

> Other firms were cutting hiring of new graduates on the grounds that AI could now do their work, and Cloudflare's view was blunt: "we think this misreads the moment completely, so we're heading in the opposite direction."

Cloudflare blog, "Cloudflare's 1,111 intern program", 22 September 2025. https://blog.cloudflare.com/cloudflare-1111-intern-program/

**Note 2.**

> Senior employment "showed no sign of a break in trend." As in the Stanford study, the decline was "driven primarily by slower hiring," with little sign of more people leaving.

Hosseini and Lichtinger, "Generative AI as Seniority-Biased Technological Change", May 2026 version (working paper; SSRN 5425555), from the author's site. https://raw.githack.com/s-mahdihosseini/Website/b99fa2962dcc4c165bbc3c41dd283afa99c5ccfb/GenAI_SenBTC_May_2026.pdf

**Note 3.**

> The adopters were few, about 3.7% of the firms, but they employed roughly 16% of all the workers in the data.

Hosseini and Lichtinger (May 2026 version).

**Note 4.**

> Ranking juniors by the prestige of their university, the authors find that "juniors from mid-tier universities experienced the largest relative declines," while graduates of the top and bottom tiers saw smaller falls.

Hosseini and Lichtinger (May 2026 version), footnote 6 and Supplemental Appendix A.19.

**Note 5.**

> Revelio Labs, which tracks the labour market, reported in July 2026 that American postings for entry-level jobs had fallen about 35% since early 2023, and added its own warning that "the decline in job postings alone does not establish AI as the cause."

Revelio Labs, July 2026. https://www.reveliolabs.com/blog/fast-company-entry-level-hiring

**Note 6.**

> In mid-2026 about 42% of recent graduates were working in jobs that don't usually need a degree, a share the bank calls underemployment.

Federal Reserve Bank of New York, "The Labor Market for Recent College Graduates", data series (seasonally adjusted, three-month moving average): June 2026 unemployment 5.698% (recent graduates) and 4.061% (all workers); September 2022 4.016% and 3.427%; underemployment 41.95% in June 2026 and 42.26% in December 2025. The release of 6 August 2026 says underemployment "edged up to 42 percent". https://www.newyorkfed.org/research/college-labor-market

**Note 7.**

> For every apprentice these employers hired, they hired 1.8 graduates, down from 2.3 the year before.

Institute of Student Employers, "Apprenticeships rise as graduate vacancies drop 8%", 2025. https://ise.org.uk/knowledge/insights/492/apprenticeships_rise_as_graduate_vacancies_drop_8/

**Note 8.**

> A year later the same body found graduate hiring up 4%, or just 0.8% leaving out a few unusual employers.

Institute of Student Employers, "What the stabilised graduate market really looks like", 2026. https://ise.org.uk/knowledge/insights/617/what_the_stabilised_graduate_market_really_looks_like

**Note 9.**

> The Budget Lab at Yale found in October 2025 that "the broader labor market has not experienced a discernible disruption since ChatGPT's release 33 months ago." It added that the gap facing young graduates "could also simply reflect a slowing labor market."

The Budget Lab at Yale, 1 October 2025. https://budgetlab.yale.edu/research/evaluating-impact-ai-labor-market-current-state-affairs

**Note 10.**

> Their main explanation is "the sharpest monetary policy tightening cycle in four decades."

Iscenko and Curto Millet, working paper published by the Economic Innovation Group, January 2026. https://eig.org/wp-content/uploads/2026/01/TAWP-Iscenko-Millet.pdf

**Note 11.**

> Their main explanation is "the sharpest monetary policy tightening cycle in four decades." And Fairlie and Wu, at UCLA, found that recent graduates' unemployment "did not spike in summer 2026" compared with earlier summers, and "did not rise in a significant way relative to older college graduates."

Fairlie and Wu, IZA Discussion Paper 18945, September 2026. https://econpapers.repec.org/RePEc:iza:izadps:dp18945

**Note 12.**

> The promoted workers had "significantly better performance for the first two years." The outside hires also left more often: they were about 61% more likely to be pushed out and 21% more likely to quit.

Bidwell, "Paying More to Get Less", *Administrative Science Quarterly* 56(3), 2011. The exit figures are differences in hazard rates. https://wpa.wharton.upenn.edu/wp-content/uploads/2016/02/Administrative_Science_Quarterly-2011-00018392114335621.pdf

**Note 13.**

> For about 28% of apprentices, the work they did was worth more than their gross cost.

BIBB (Bundesinstitut für Berufsbildung), press release on the 2017/18 cost-benefit survey (in German). https://www.bibb.de/de/pressemitteilung_123901.php

**Note 14.**

> As reported in a UC Santa Barbara release, residents got "ten to twenty times less practice." The robot "allowed an expert to operate alone", and so "the trainee was optional."

UC Santa Barbara College of Engineering, "Shining a light on shadow learning", quoting Beane on his study in *Administrative Science Quarterly* (2019); the article itself was not read. https://www.engineering.ucsb.edu/news/shining-light-shadow-learning

**Note 15.**

> Matt Garman, who runs Amazon's cloud business, said in August 2025, in remarks reported by *The Register*, that replacing juniors with AI was "the dumbest thing I've ever heard." Juniors, he said, are "probably the least expensive employees you have," and he asked: "How's that going to work when ten years in the future you have no one that has learned anything."

*The Register*, 21 August 2025, reporting Garman's video interview with Matthew Berman. https://www.theregister.com/2025/08/21/aws_ceo_entry_level_jobs_opinion/

**Note 16.**

> Matt Garman, who runs Amazon's cloud business, said in August 2025, in remarks reported by *The Register*, that replacing juniors with AI was "the dumbest thing I've ever heard." Juniors, he said, are "probably the least expensive employees you have," and he asked: "How's that going to work when ten years in the future you have no one that has learned anything." IBM's head of human resources, Nickle LaMoreaux, put it the same way in 2026: "If we don't continue to invest in entry-level hires, what happens in 3-5 years? ... There's no pipeline; the well simply dries up."

A. McConnon, "The bottom rung returns as AI reshapes entry-level jobs", IBM Think, March 2026. https://www.ibm.com/think/news/entry-level-roles-get-reset-ai

**Note 17.**

> Nine years after starting, they earned on average $5,839 a year more than similar people who hadn't joined, and an estimated $98,718 more over a career.

Reed et al. (Mathematica, for the US Department of Labor), study of Registered Apprenticeship in 10 states, July 2012 (read via the Internet Archive). Completers: $240,037 over a career. https://web.archive.org/web/20250113102729/https://www.dol.gov/sites/dolgov/files/ETA/publications/ETAOP_2012_10.pdf

**Note 18.**

> Of the employers interviewed, two-thirds had recouped their investment and one-third had not.

Abt Global, "Do Employers Earn Positive Returns to Investments in Apprenticeship?", 28 October 2022 (American Apprenticeship Initiative). https://www.abtglobal.com/insights/publications/report/do-employers-earn-positive-returns-to-investments-in-apprenticeship

**Note 19.**

> In Switzerland, more than 60% of firms found apprenticeships profitable.

Muehlemann and Wolter, "Return on investment of apprenticeship systems for enterprises", *IZA Journal of Labor Policy* 3:25 (2014). https://doi.org/10.1186/2193-9004-3-25

**Note 20.**

> Agents with two months on the job and the AI assistant performed as well as agents with more than six months who didn't have it.

Brynjolfsson, Li and Raymond, "Generative AI at Work", arXiv version 2 (November 2024). https://arxiv.org/pdf/2304.11771

**Note 21.**

> The same study found that among agents in their first six months, quitting fell by about 10 percentage points, from a base of about 25%.

Brynjolfsson, Li and Raymond (arXiv v2, 2024): a fall of about 10 percentage points, or 40%, among agents with under six months' tenure; the authors note the estimate lacks agent fixed effects.

**Note 22.**

> In a 2025 survey of 319 knowledge workers by researchers at Microsoft and Carnegie Mellon, "higher confidence in GenAI is associated with less critical thinking."

Lee et al. (Microsoft Research and Carnegie Mellon), CHI 2025. https://advait.org/files/lee_2025_ai_critical_thinking_survey.pdf

**Note 23.**

> Natasha Pillay-Bemath, who leads IBM's global talent acquisition, said entry-level roles "are shifting from purely task-driven work to analysis, problem-solving and responsible AI use." With AI taking more of the routine coding and documentation, juniors are expected to understand "systems end-to-end" and to spend time "validating AI outputs for quality and bias," and "entry-level developers are now working with real clients far earlier in their careers."

McConnon, IBM Think, March 2026. The page attributes the "triple" plan to LaMoreaux. https://www.ibm.com/think/news/entry-level-roles-get-reset-ai

**Note 24.**

> Shopify, as reported by the hiring firm CoderPad, plans to grow from about 100 interns a year to about 1,000.

CoderPad, interview with Shopify's Farhan Thawar (no Shopify statement found). https://coderpad.io/blog/hiring-developers/in-the-ai-era-shopify-is-investing-in-junior-engineers-not-cutting-them/

## Chapter 12: The Jevons Scorecard

**Note 1.**

> When the same executives talked about productivity from anything else, about three-quarters of the sentences looked ahead.

Ozkan, Kalyani and Sullivan, "AI and Productivity: What Firms Are Saying on Earnings Calls", Federal Reserve Bank of St. Louis, *On the Economy*, 31 July 2026. https://www.stlouisfed.org/on-the-economy/2026/jul/ai-productivity-what-firms-say-earnings-calls

**Note 2.**

> The executives said AI had raised their annual labour productivity growth by 0.2% over the last three years, "a modest impact", and they expected a boost of 0.6% a year over the next three.

Yotzov, Barrero, Bloom, Bunn, Davis, Meyer et al., "Firm Data on AI", NBER Working Paper 34836 (February 2026, revised October 2026), working-paper version. Earlier versions report about 6,000 executives and different figures. The 78% averages seven surveys; the US, UK, German and Mexican results are employment-weighted (the paper's note to Figure 4A), and the US figure alone is 95%. The US survey is the Atlanta Fed's Survey of Business Uncertainty. The paper's first version put US adoption at 78%, counting firms that skipped the question as non-users; the current draft drops those firms, which gives 94% for November 2025 and 95% for June 2026 (footnote 13). https://www.nber.org/system/files/working_papers/w34836/w34836.pdf

**Note 3.**

> Their name for it is "a productivity paradox, in which perceived productivity gains are larger than measured productivity gains, likely reflecting a delay in revenue realizations."

Baslandze, Edwards, Graham, McClure, Meyer, Sparks, Waddell and Weitz, "Artificial Intelligence, Productivity, and the Workforce: Evidence from Corporate Executives", NBER Working Paper 34984, March 2026 (Duke/Richmond Fed and Atlanta Fed CFO Survey). https://www.nber.org/system/files/working_papers/w34984/w34984.pdf

**Note 4.**

> American labour productivity rose 2.1% from 2024 to 2025, and the official figure says nothing about how much, if any, came from AI.

US Bureau of Labor Statistics, Productivity and Costs, revised fourth-quarter 2025 release, 24 March 2026: nonfarm business labour productivity, annual average, 2024 to 2025. The preliminary release said 2.2%. https://www.bls.gov/news.release/archives/prod2_03242026.htm

**Note 5.**

> In 1987 the economist Solow wrote, in a book review, that one "can see the computer age everywhere but in the productivity statistics."

R. Solow, "We'd Better Watch Out", *New York Times Book Review*, 12 July 1987, as quoted in Brynjolfsson, Rock and Syverson, "The Productivity J-Curve", NBER Working Paper 25148 (revised January 2020). The original was not read. https://www.nber.org/system/files/working_papers/w25148/w25148.pdf

**Note 6.**

> It took about two more decades for half of factory drive to be electrified, and factory productivity didn't show the effect until the early 1920s, "four decades after the first central power station opened for business." When it came, it came hard: about half of a 5-percentage-point jump in the growth of manufacturing productivity in the 1920s was accounted for, statistically, by the growth of electric motors in factories.

P. A. David, "The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox", *American Economic Review* 80(2), May 1990, pp. 355-361. Quoted from a scanned copy of the journal pages, including David's "group drive" and "unit drive". https://www.gwern.net/doc/economics/automation/1990-david.pdf

**Note 7.**

> The economists Brynjolfsson, Rock and Syverson put it this way: "it took a generation for the nature of factory layouts to be re-invented."

Brynjolfsson, Rock and Syverson, NBER w25148 (revised January 2020). https://www.nber.org/system/files/working_papers/w25148/w25148.pdf

**Note 8.**

> They call the shape a J-curve.

Brynjolfsson, Rock and Syverson, NBER w25148, abstract; published in *American Economic Journal: Macroeconomics* 13(1), 2021 (the published text was not read). https://www.nber.org/system/files/working_papers/w25148/w25148.pdf

**Note 9.**

> The authors trace the loss to the costs of adjusting, which they can see in the data: more half-finished inventory, more robots bought, workers let go.

McElheran, Yang, Kroff and Brynjolfsson, "The Rise of Industrial AI in America: Microfoundations of the Productivity J-curve(s)", preliminary draft, December 2025, US Census data on manufacturing, 2017 and 2021. Their instrumental-variable estimates are much larger, and the authors say these apply to firms at the margin of adopting and are not representative of digitally advanced firms. https://extranet.sioe.org/uploads/sioe2026/mcelheran-2026-01-15_6085.pdf

**Note 10.**

> In the study of pre-chatbot AI investment that chapter 8 described, the sales gains took about two to three years to arrive.

T. Babina and A. Fedyk, "The effects of AI on firms and workers", Brookings, 1 July 2025. https://www.brookings.edu/articles/the-effects-of-ai-on-firms-and-workers/

**Note 11.**

> About 2.3% said it had gone up, and 2.0% said it had gone down.

Bonney, Breaux, Dinlersoz, Foster, Haltiwanger and Pande, "The Microstructure of AI Diffusion: Evidence from Firms, Business Functions, and Worker Tasks", NBER Working Paper 35141 / CES WP 26-25, April 2026, table 4 (firm-weighted; Business Trends and Outlook Survey, November 2025 to January 2026). https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 12.**

> But about 15% had hired fewer people because of it, and about 13% had hired more.

Abel, Deitz, Emanuel and Montalbano, "Businesses Are Using AI to Transform Work, Not Cut Jobs", Federal Reserve Bank of New York, *Liberty Street Economics*, 1 September 2026. Firms in New York and northern New Jersey; self-reported. The post's chart labels these as shares of AI users; the text calls them shares of service firms. https://libertystreeteconomics.newyorkfed.org/2026/09/businesses-are-using-ai-to-transform-work-not-cut-jobs/

**Note 13.**

> The Yotzov survey found "considerable job churn" across seven countries with essentially no net effect: more than 40% of firms expected AI to move their headcount up or down, in ways that "roughly offset only in the aggregate."

Yotzov et al., NBER w34836 (revised October 2026), abstract. https://www.nber.org/system/files/working_papers/w34836/w34836.pdf

**Note 14.**

> Of the firms using AI, 64% reported no change to how they were organised: about 15% had trained staff and about 15% had built new workflows.

Bonney et al., NBER w35141 (April 2026). https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 15.**

> The heavier AI investors saw their sales and their workforces grow more quickly, mostly through new products.

T. Babina, A. Fedyk, A. He and J. Hodson, "Artificial intelligence, firm growth, and product innovation", *Journal of Financial Economics* 151 (2024), 103745, abstract; sizes in Babina and Fedyk, Brookings, 1 July 2025. https://ideas.repec.org/a/eee/jfinec/v151y2024ics0304405x2300185x.html

**Note 16.**

> The same authors found no clear effect yet on jobs or wages across whole occupations or industries.

Acemoglu, Autor, Hazell and Restrepo, "AI and Jobs: Evidence from Online Vacancies", NBER Working Paper 28257 (revised February 2022), table 5 (Felten et al. exposure measure; vacancies 2010 to 2018); published in *Journal of Labor Economics* 40(S1), 2022. https://www.nber.org/system/files/working_papers/w28257/w28257.pdf

**Note 17.**

> Firms that built AI into their business functions were also more likely to report sales growth, by 3.5 percentage points, and slightly more likely to report falling employment, by about 0.8 to 0.9 points.

Bonney et al., NBER w35141 (April 2026): self-reported outcomes, correlations; baselines about 13% (sales growth) and 9-10% (employment declines). https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 18.**

> Cutting costs alone was a weaker match.

Baslandze et al., NBER w34984 (March 2026). https://www.nber.org/system/files/working_papers/w34984/w34984.pdf

**Note 19.**

> The same report, by People Matters, said AI agents were working a backlog of more than 100 million sales leads left uncalled over 26 years.

People Matters, "Salesforce cuts 4,000 support jobs as AI takes the lead, says CEO", 1 September 2025 (updated 3 September), reporting Benioff's remarks on The Logan Bartlett Show. https://www.peoplematters.in/news/strategic-hr/salesforce-cuts-4000-support-jobs-as-ai-takes-the-lead-says-ceo-43231

**Note 20.**

> A day later a company spokesperson told KTVU, a San Francisco television station, that Salesforce no longer needed "to actively backfill support engineer roles" and had "successfully redeployed hundreds of employees into other areas like professional services, sales, and customer success." The spokesperson gave no number.

KTVU, 2 September 2025, quoting a Salesforce spokesperson. No company release giving the number was found. https://www.ktvu.com/news/salesforce-ai-layoffs-marc-benioff

**Note 21.**

> Fortune added, relaying *Business Insider*, that Salesforce had cut fewer than 1,000 roles that February.

Fortune, 27 April 2026, quoting Benioff's post on X; the February cuts are Fortune relaying *Business Insider*. https://www.fortune.com/2026/04/27/salesforce-ceo-marc-benioff-hiring-1000-new-grads-ai-jobs/

**Note 22.**

> But among firms that did substitute, the share replacing "a large number" of tasks rose from 2.5% to 7% between the two Census surveys, though the second asked its question differently.

Bonney et al., NBER w35141 (April 2026), body text. The abstract's "66%" counts only firms with some task effect. The earlier survey is Bonney et al., NBER Working Paper 32319 (April 2024). https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 23.**

> The Census authors say their survey cannot yet see "AI-driven changes to hiring practices", and a question on hiring is planned but not yet approved.

Bonney et al., NBER w35141 (April 2026), text and footnote 31. https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 24.**

> Across all American workers, the share of work hours saved with AI's help grew from 1.6% to 2.2% between late 2024 and mid-2026, by one tracker's estimate.

Bick, Blandin and Deming, Generative AI Adoption Tracker, as reported on the FRED Blog, "Does generative AI save time at work?", 27 August 2026: third quarter of 2024 to second quarter of 2026, all employed adults. An earlier 2025 estimate from the same team was revised. https://fred.stlouisfed.org/blog/2026/08/does-generative-ai-save-time-at-work/

**Note 25.**

> Klarna, whose story chapter 10 tells, said its revenue per employee had reached $1.24 million in 2025, up 3.6 times since 2022, with headcount down 49% over the same years.

Klarna press release on full-year 2025 results, 19 February 2026: "Revenue per employee reached $1.24 million, up 3.6 times since 2022 as headcount declined 49%." https://www.klarna.com/international/press/klarna-accelerates-u-s-growth-and-delivers-usd1bn-revenue-driven-by-rapid/

**Note 26.**

> In May 2025, as that chapter recounts, its chief executive was reported as saying that the AI-first path was not the right one, while its own release that month said customer satisfaction had held.

*Entrepreneur*, 9 May 2025, relaying Siemiatkowski's interview with Bloomberg ("wasn't the right path" is the reporter's paraphrase); and Klarna's press release on first-quarter 2025 results, 19 May 2025 ("whilst maintaining customer satisfaction levels"). https://www.entrepreneur.com/business-news/klarna-ceo-reverses-course-by-hiring-more-humans-not-ai/491396 https://www.klarna.com/international/press/klarna-accelerates-global-momentum-in-q1-2025-and-unlocks-large-gains-from/

**Note 27.**

> The Atlanta Fed's survey of firms, weighted by employment, put adoption at around 78% in its November 2025 round.

J. S. Allen, "Monitoring AI Adoption in the U.S. Economy", FEDS Notes, Federal Reserve Board, 3 April 2026: Census BTOS (firm-weighted) and the Atlanta Fed Survey of Business Uncertainty (employment-weighted); the note puts the gap down to weighting, sampling and question wording. The employment-weighted Census figure of 32% is from Bonney et al., NBER w35141 (April 2026). The note's SBU figure ("around 78 percent") comes from the survey's November 2025 AI questions, the same survey Yotzov et al. use for the US (note 2). https://www.federalreserve.gov/econres/notes/feds-notes/monitoring-ai-adoption-in-the-u-s-economy-20260403.html https://www.nber.org/system/files/working_papers/w35141/w35141.pdf

**Note 28.**

> **Surveys change their questions.** In late 2025 the Census survey changed its question from AI used "in producing goods or services" to AI used in "any of its business functions", so the two rounds can't be compared directly.

Allen, FEDS Notes (3 April 2026); Bonney et al., NBER w35141, footnote 29. https://www.federalreserve.gov/econres/notes/feds-notes/monitoring-ai-adoption-in-the-u-s-economy-20260403.html

## Chapter 13: Where the Other Jobs Come From

**Note 1.**

> Across all its members, more than before raised a shortage of workers without being asked.

Associated Builders and Contractors, press release on its member survey (conducted 20 August to 4 September 2026), 15 September 2026, quoting chief economist Anirban Basu: "Data centers continue to keep contractors busy even as activity softens in other segments. Although the backlog gap between contractors with and without data center work narrowed in August (9.9 vs. 8.3 months, respectively), that appears to reflect more contractors securing work in the data center segment rather than a broader structural trend. Roughly 1 in 6 ABC members is currently under contract to work on a data center, the highest proportion on record." He added that there was "a sharp increase in the number of contractors who, unprompted, mentioned labor shortages in the survey." Cached copy: sources/cache/text/d4aaa1a766db.txt. Moved 2026-10-22 from route one to the chapter's opening; the label stays [^14], so it prints as note 1. https://www.abc.org/News-Media/News-Releases/abc-survey-1-in-6-members-perform-data-center-work-backlog-rebounds-in-august (retrieved 2026-10-22).

**Note 2.**

> There are about 51,000 more, a gap of 13.6%.

BLS, Current Employment Statistics, CES4422110001 (electric power generation, transmission and distribution, NAICS 2211, seasonally adjusted, thousands), https://data.bls.gov/timeseries/CES4422110001?from_year=2010&to_year=2026&output_view=data&include_graphs=false, retrieved 2026-10-22. Our calculation, analysis/part3/t1_t6/analyze.py, results in analysis/results_part3_t1_t6.json: average September 2025 to August 2026 426.2k against a 2015-2019 straight-line trend of 375.2k, gap +13.6% [95% interval 12.0 to 15.1]; trend slope about -2k a year. Research note: research_notes/part3-buildout-research-it.md §1.

**Note 3.**

> Since December 2022, its payroll has grown by 8.9%.

As note 1. The gap in calendar 2022 (+1.8%) is an exploratory figure added after the results were seen, labelled so in analysis/results_part3_t1_t6.json. The +8.9% change since December 2022 is from our red-team review (not part of the original plan), "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1 table (rt_t1_t6.json), which also uses the long CES series 1990-2026 in analysis/part3/redteam/data/ces_long.csv.

**Note 4.**

> And in the decades before AI, a straight line carried this far ahead had missed by as much as this in about one period in four.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1, point 2: natural-gas distribution (NAICS 2212) +11.8% above its 2015-19 trend (+4.8% in 2022), water utilities +4.3%; candidates named there: grid and pipeline replacement, retirements and rehiring, IRA-funded investment (enacted August 2022); 2211 gap rose 11.8 points after 2022 against 7.0 for gas. Same-horizon comparison: 19 overlapping pre-AI trend windows (1990-2008), 5 of 19 missed by at least as much as 2211 (rank p 0.30). Not pre-registered.

**Note 5.**

> The file records the few things we had glimpsed while checking file layouts before every detail was fixed.

Our pre-registration, "Pre-registration: the book's own tests (Part 3)", analysis/PREREGISTRATION.md (commit 93726bb, 22 October 2026, written before any of the tests was run and before most of their data were downloaded; the OEWS tables had been cached earlier for other chapters, and the T4/T5 files were downloaded before every detail was fixed). Its "Deviations" section records, with dates, the implementation details fixed before results, the few raw values seen while checking file layouts (a few NAICS 54 application counts, 2010-2013 values of NAICS 518, OEWS file layouts), and, labelled separately, the additions made after the results were seen.

**Note 6.**

> Then a separate reviewer, our red team, tried to break every result, in both directions, and we report what survived.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md. None of it was part of the original plan (not pre-registered); it challenges the pre-registered results and does not replace them.

**Note 7.**

> Power-line construction was 10.6% below (12.6 to 8.3 below), electricians 8.6% below (11.0 to 6.1 below), and semiconductors 2.9% below, with an interval running from 7.4 below to 2.6 above.

BLS, Current Employment Statistics, series CES4422110001 (https://data.bls.gov/timeseries/CES4422110001?from_year=2010&to_year=2026&output_view=data&include_graphs=false), CES5051800001 (https://data.bls.gov/timeseries/CES5051800001?from_year=2010&to_year=2026&output_view=data&include_graphs=false), CES2023713001 (https://data.bls.gov/timeseries/CES2023713001?from_year=2010&to_year=2026&output_view=data&include_graphs=false) and CES3133440001 (https://data.bls.gov/timeseries/CES3133440001?from_year=2010&to_year=2026&output_view=data&include_graphs=false), retrieved 2026-10-22; and BLS, Occupational Employment and Wage Statistics (OEWS), national May tables, via Wayback Machine copies of bls.gov, e.g. https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip (May 2025) and https://web.archive.org/web/20240522032635id_/https://www.bls.gov/oes/2022/may/oes_nat.htm (May 2022); full list in analysis/data/part3/t1_t6/SOURCES.md and analysis/data/part3/t4_t5/SOURCES.md, electricians 47-2111. Our calculation, analysis/part3/t1_t6/analyze.py; analysis/results_part3_t1_t6.json. Gaps in % of the 2015-2019 trend, latest 12 months (OEWS: May 2025): 2211 +13.6 [12.0, 15.1]; 518 +9.4 [7.9, 11.4]; 23713 -10.6 [-12.6, -8.3]; electricians -8.6 [-11.0, -6.1]; 3344 -2.9 [-7.4, 2.6]. Intervals: moving-block bootstrap of trend residuals, 10,000 resamples, seed 20261022; they cover uncertainty in the line only.

**Note 8.**

> But today's gaps sit six or seven years past the end of their lines, and lines drift further the longer they run, so that comparison was too short to judge either way.

Our pre-registration, "Pre-registration: the book's own tests (Part 3)", analysis/PREREGISTRATION.md (commit 93726bb, 22 October 2026, written before any of the tests was run and before most of their data were downloaded; the OEWS tables had been cached earlier for other chapters, and the T4/T5 files were downloaded before every detail was fixed), T1 placebo (trend 2012-2016, gap over 2017-2019) and verdict rule; by it 2211 and 518 support, 23713, 3344 and electricians go against (analysis/results_part3_t1_t6.json). Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1 "Why it is needed" (not part of the original plan): the planned comparison measures 0-3 years after its trend window, the main test 6-7 years after (69-81 months). Planned comparison for 5415 (computer systems design): -2.8% [-3.7, -1.8].

**Note 9.**

> In pre-AI history back to 1990, the red team found, lines carried the same distance missed by an average of 26 to 58 points for three of these series, and by about 9 points for electric power.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1, point 1: mean absolute same-horizon pre-AI gap 30.6 (518), 58.2 (3344), 25.9 (23713) and 8.7 points (2211). Not pre-registered. Electricians have only 5 such windows, all distorted by the housing bust, and are not counted.

**Note 10.**

> Since December 2022 its employment has fallen 6.6%.

BLS CES5051800001, https://data.bls.gov/timeseries/CES5051800001?from_year=2010&to_year=2026&output_view=data&include_graphs=false; our calculation (analysis/results_part3_t1_t6.json, exploratory 2022 gap +22.7% [21.6, 24.2]); our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1, point 3 (-6.6% since December 2022). The 2022 gap was added after the results were seen; the change since December 2022 is not part of the original plan.

**Note 11.**

> Electricians were already 8.7% below theirs in May 2022.

BLS CES2023713001, https://data.bls.gov/timeseries/CES2023713001?from_year=2010&to_year=2026&output_view=data&include_graphs=false; BLS, Occupational Employment and Wage Statistics (OEWS), national May tables, via Wayback Machine copies of bls.gov, e.g. https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip (May 2025) and https://web.archive.org/web/20240522032635id_/https://www.bls.gov/oes/2022/may/oes_nat.htm (May 2022); full list in analysis/data/part3/t1_t6/SOURCES.md and analysis/data/part3/t4_t5/SOURCES.md, electricians 47-2111 (690k May 2022, 757,220 May 2025). Our calculation, research_notes/part3-buildout-research-it.md §1; electricians' May 2022 gap -8.7% is exploratory, added after the results were seen.

**Note 12.**

> On the same method, total private employment sits 5.3% below its own line, and specialty construction trades 10.5% below.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1, point 4: total private employment -5.3% below its 2015-19 line; specialty trades -10.5%; nonresidential building -9.6%. Not pre-registered.

**Note 13.**

> Whichever way it pointed, it would be a poor test.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T1, point 5 (CHIPS Act money mostly pays construction workers, counted in construction; 3344 covers all electronic components; much of the chip supply chain abroad). Not part of the original plan (not pre-registered).

**Note 14.**

> Private spending on building US data centres ran at an annual rate of about $85 billion in August 2026 (a preliminary figure), against $8.8 billion in August 2019.

US Census Bureau, Construction Spending (C30), private construction, seasonally adjusted annual rate, "Data center", release of 1 October 2026: $84.95bn (August 2026, preliminary) against $8.8bn (August 2019). https://www.census.gov/construction/c30/xlsx/privsatime.xlsx (retrieved 2026-10-22). The "tenfold" in the text is our calculation from the same file.

**Note 15.**

> Federal statisticians project electrician jobs to grow 9% from 2025 to 2035, with about 72,700 openings a year, and name data centres among the reasons.

BLS, Occupational Outlook Handbook, "Electricians", last modified 27 August 2026: employment projected to grow 9% from 2025 to 2035, about 72,700 openings a year; names data-centre demand. https://www.bls.gov/ooh/construction-and-extraction/electricians.htm (retrieved 2026-10-22).

**Note 16.**

> Measured against the 2016-2019 pattern, the difference was +0.1%, and the range it probably lies in runs from about 10% down to about 10% up.

US Census Bureau, Business Formation Statistics, monthly, seasonally adjusted, by NAICS sector, https://www.census.gov/econ/bfs/csv/bfs_monthly.csv (release current on 2026-10-22, data to September 2026); definitions https://www.census.gov/econ/bfs/definitions.html; methodology https://www.census.gov/econ/bfs/methodology.html, series BA_HBA. Our calculation, analysis/part3/t2_t3/analysis.py; analysis/results_part3_t2_t3.json: exposed (51, 54) minus less exposed (23, 72, 81), mean of sector logs, December 2022 to September 2026 against the 2016-2019 trend: +0.1% [95% interval -10.2% to +9.6%]. Research note: research_notes/part3-newfirms-spending.md §1.

**Note 17.**

> Fit the line to a longer stretch of years, or use no line at all, and the exposed sectors fall behind.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T2: without 72, +0.090 log points; 54 alone against 23 + 81, +0.185 (about +20%); no trend -0.205; trend 2005-19 -0.115; 2010-19 -0.025. Not pre-registered.

**Note 18.**

> Taken alone, professional services applications rose about 21% above their own trend, but restaurants and hotels rose 32%, and information barely moved.

US Census Bureau, Business Formation Statistics, monthly, seasonally adjusted, by NAICS sector, https://www.census.gov/econ/bfs/csv/bfs_monthly.csv (release current on 2026-10-22, data to September 2026); definitions https://www.census.gov/econ/bfs/definitions.html; methodology https://www.census.gov/econ/bfs/methodology.html; our calculation (analysis/results_part3_t2_t3.json), each sector against its own 2016-2019 trend, description only: professional services +21.5% (8.8 to 31.9); accommodation and food +31.9% (24.0 to 37.3); information +0.5% (-18.7 to 21.0).

**Note 19.**

> And it is a forecast from a model, weighting each application by its predicted chance of hiring; the count of firms that actually hired runs only as far as applications made in December 2022.

US Census Bureau, Business Formation Statistics, monthly, seasonally adjusted, by NAICS sector, https://www.census.gov/econ/bfs/csv/bfs_monthly.csv (release current on 2026-10-22, data to September 2026); definitions https://www.census.gov/econ/bfs/definitions.html; methodology https://www.census.gov/econ/bfs/methodology.html, series BF_PBF4Q (projected employer business formations within 4 quarters). Our calculation: +12.1% [-3.3%, +24.6%], mean of sector logs. Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T2: other trend choices -0.016 to +0.042 log points; by year 2023 -0.014, 2024 +0.048, 2025 +0.159, 2026 (Jan-Sep) +0.328; projected formations per application rose in 51, 54 and also 81. Counted formations (BF_BF4Q) end with December 2022 applications (Census BFS methodology page, read 2026-10-22). By the pre-registered T2 rule the secondary counts as support, a pass (analysis/results_part3_t2_t3.json, BF_PBF4Q_meanlog verdict_for_book: true). The red-team checks are not part of the original plan.

**Note 20.**

> A Census working paper by Dinlersoz, Dogan and Zolas, published in March 2024, fits that cautious reading: it found applications for AI-related businesses jumping in 2023, and those firms more likely to become employers but less likely to survive.

Dinlersoz, Dogan and Zolas, "Starting Up AI", US Census Bureau, Center for Economic Studies Working Paper 24-09, March 2024. https://census.gov/library/working-papers/2024/adrm/CES-WP-24-09.html (retrieved 2026-10-22).

**Note 21.**

> The correlation was -0.015, and the range it probably lies in runs from -0.27 to 0.28.

BEA, NIPA Tables 2.4.5 (Personal Consumption Expenditures by Type of Product) and 2.4.4 (price indexes), annual, flat files at https://apps.bea.gov/national/Release/TXT/ (NipaDataA.txt), retrieved 2026-10-22. Our calculation, analysis/part3/t2_t3/analysis.py: 70 detailed PCE lines, 1959-2019, Pearson correlation between change in log relative price and change in log spending share r = -0.015 [95% interval -0.27, 0.28], permutation p = 0.90; slope -0.017 (implied elasticity of substitution about 1). analysis/results_part3_t2_t3.json.

**Note 22.**

> On the plain average they didn't, and a forecast built on the 1959-1999 pattern predicted 2000-2019 worse than assuming nothing changed.

Our calculation, analysis/results_part3_t2_t3.json: the 1959-1999 relationship predicts 2000-2019 share changes with skill -0.42 [95% interval -1.22, 0.04] against a no-change forecast (pre-registered out-of-sample check).

**Note 23.**

> Weighting each category by its size tilts the result: cheaper categories then tended to lose some share.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T3-A: weighted by 2019 spending, slope +0.25 [0.02, 0.68]; by 1959 spending +0.18 [-0.03, 0.53]; robust and trimmed versions about +0.17 to +0.25. Not pre-registered.

**Note 24.**

> The rank correlation across 18 matched categories was 0.67, with a range from 0.25 to 0.89.

BEA, NIPA Tables 2.4.5 (Personal Consumption Expenditures by Type of Product) and 2.4.4 (price indexes), annual, flat files at https://apps.bea.gov/national/Release/TXT/ (NipaDataA.txt), retrieved 2026-10-22; BLS CES annual averages for the matched industries (pages listed in analysis/data/part3/t2_t3/SOURCES.md); match table analysis/part3/t2_t3/match_table.csv, written before results. Our calculation: Spearman rho 0.67 [95% interval 0.25, 0.89], 18 categories, 1990-2019, permutation p = 0.0025. Chart: analysis/part3/t2_t3/charts/t3_spending_jobs.png.

**Note 25.**

> It holds when any single category is dropped, with the correlation staying between 0.60 and 0.75, and it holds at 0.64 without health care, medicines and social services.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T3-B: leave-one-out rho 0.60 to 0.75; without health care, pharmaceuticals and social services 0.64. Not pre-registered.

**Note 26.**

> It is also the only result that still passes when all our tests are judged together under a stricter standard, as chapter 14 explains.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, "Multiple comparisons" (Holm correction across the six tests with same-horizon benchmarks for T1): only T3-B survives (p = 0.0025). Not pre-registered. Chapter 14 explains the method.

**Note 27.**

> Every category that gained both spending and jobs share also got more expensive relative to other things.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T3-B: health care +0.27 log points of relative price, education +0.94, recreation +0.21, social services +0.25, food services +0.21, housing +0.26. Not part of the original plan (not pre-registered).

**Note 28.**

> And across the 18, the link between rising price and rising share is only suggestive.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T3-B and T3-A point 3: 14 of 18 categories got relatively dearer; across the 18, relative price and spending-share change r = +0.44 [0.03, 0.75], permutation p = 0.07 ("suggestive"); labour is most of the cost in these services. Not part of the original plan (not pre-registered).

**Note 29.**

> On any version of our numbers, a large cut in the price of professional services would move little spending either way, tens of billions of dollars at most, next to a consumer economy of about $20 trillion; chapter 14 gives the range.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T3 projection: at a 40% relative price cut in professional services, the pre-registered interval runs from a $59bn loss to a $51bn gain in freed spending; spending-weighted or trimmed slopes give $32-36bn freed; tens of billions at most either way, all small next to roughly $20 trillion of consumer spending. Our projection in research_notes/part3-newfirms-spending.md §2 (data to 2025). Not part of the original plan (not pre-registered).

**Note 30.**

> From 1990 to 2019, about 39% of the gains in budget share among our 18 categories went to health care, 19% to medicines, 18% to finance and insurance and 10% to recreation.

BEA, NIPA Tables 2.4.5 (Personal Consumption Expenditures by Type of Product) and 2.4.4 (price indexes), annual, flat files at https://apps.bea.gov/national/Release/TXT/ (NipaDataA.txt), retrieved 2026-10-22; our calculation (research_notes/part3-newfirms-spending.md §2): shares of the 1990-2019 gains in spending share among the 18 matched categories: health care 39%, medicines 19%, finance and insurance 18%, recreation 10%, social services 5%, education 4.5%, housing 3%. Description of history, not a forecast.

**Note 31.**

> Most of the rise came before AI: the industry went from about 732,000 jobs in 2019 to about 893,000 in 2022, edged up to about 934,000 in 2024, and has slipped back since.

BLS CES6054170001 (scientific research and development services, NAICS 5417), https://data.bls.gov/timeseries/CES6054170001?from_year=2010&to_year=2026&output_view=data&include_graphs=false. Our calculation, analysis/results_part3_t1_t6.json: 913.2k against trend 828.7k, +10.2% [3.1, 19.2]; annual averages 732k (2019), 893k (2022), 929k (2023), 934k (2024, the highest), 922k (2025), 914k (2026, January-September), from the long CES series in analysis/part3/redteam/data/ces_long.csv. Description; no test (T6). Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T6, and analysis/part3/redteam/rt_t1_t6.json (CES6054170001): at the same distance, 8 of 19 pre-AI windows (1990-2008) missed by at least 10.2 points in absolute terms (share 0.421; same-horizon rank p 0.45). Not part of the original plan (not pre-registered).

**Note 32.**

> Scientists counted by occupation, wherever they work, moved later: they were at their old line in May 2022 and 6.6% above it by May 2025, a figure that rests on five yearly points and on joining two versions of the occupation codes.

BLS, Occupational Employment and Wage Statistics (OEWS), national May tables, via Wayback Machine copies of bls.gov, e.g. https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip (May 2025) and https://web.archive.org/web/20240522032635id_/https://www.bls.gov/oes/2022/may/oes_nat.htm (May 2022); full list in analysis/data/part3/t1_t6/SOURCES.md and analysis/data/part3/t4_t5/SOURCES.md, major group 19-0000, harmonised to SOC 2010 by removing 19-5011 and 19-5012 from 2019 on (PREREGISTRATION deviations). Our calculation: gap -1.4% (May 2022, exploratory) and +6.6% [4.3, 9.3] (May 2025). The May 2022 gap was added after the results were seen.

**Note 33.**

> The link is a correlation; it doesn't show that AI caused either.

Hao, Xu, Li and Evans, "Artificial intelligence tools expand scientists' impact but contract science's focus", Nature, 14 January 2026: 3.02 times as many papers, 4.84 times as many citations, topics narrowed by 4.63%; correlational. https://www.nature.com/articles/s41586-025-09922-y (retrieved 2026-10-22).

**Note 34.**

> In May 2025, in a statement on its economics department's site, MIT said it had "no confidence in the provenance, reliability or validity of the data", and asked for the paper to be withdrawn. arXiv's administrators withdrew it.

MIT Department of Economics, "Assuring an accurate research record", 16 May 2025: MIT "has no confidence in the provenance, reliability or validity of the data and has no confidence in the veracity of the research contained in the paper"; MIT "has contacted arXiv to formally request that the paper be withdrawn". https://economics.mit.edu/news/assuring-accurate-research-record. arXiv record of arXiv:2412.17866 (Toner-Rodgers, "Artificial Intelligence, Scientific Discovery, and Product Innovation"; abstract describes a materials discovery technology in the R&D lab of a large US firm): "This paper has been withdrawn by arXiv Admin"; v1 21 December 2024, v2 (withdrawn) 20 May 2025. https://arxiv.org/abs/2412.17866 (both retrieved 2026-10-22).

**Note 35.**

> We scored every occupation on two measures from O\*NET, the federal government's database of what jobs involve: how much contact with other people the job requires, and how much it involves helping and caring for others.

O*NET 31.0 Database (August 2026 release), Work Context 4.C.1.a.4 "Contact With Others" and Work Activities 4.A.4.a.5 "Assisting and Caring for Others", https://www.onetcenter.org/dl_files/database/db_31_0_text.zip, licence CC BY 4.0 (https://www.onetcenter.org/license_db.html). Score: mean of the z-scores of the two; our calculation, analysis/part3/t4_t5/analyse.py.

**Note 36.**

> So the increase was about 1.23 points, with a range from just below zero to 2.5, and that fell just short of the standard we fixed beforehand.

BLS, Occupational Employment and Wage Statistics (OEWS), national May tables, via Wayback Machine copies of bls.gov, e.g. https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip (May 2025) and https://web.archive.org/web/20240522032635id_/https://www.bls.gov/oes/2022/may/oes_nat.htm (May 2022); full list in analysis/data/part3/t1_t6/SOURCES.md and analysis/data/part3/t4_t5/SOURCES.md. Our calculation, analysis/results_part3_t4_t5.json: most minus least person-facing fifth, May 2022 to May 2025, +2.57 pp a year [1.23, 3.99]; May 2016 to May 2019 +1.34; main minus placebo +1.23 [-0.08, 2.53]. Pre-registered verdict: not supported. Research note: research_notes/part3-occupations.md, T5.

**Note 37.**

> The red team found it held without health care, within broad occupation groups and in the shorter window from 2023 to 2025.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T5: without health care +2.23 [0.72, 3.91] (main minus placebo +1.68 [0.19, 3.25]); continuous score with major-group fixed effects +0.85 [0.33, 1.55] per SD; May 2023 to May 2025 +2.91 [1.71, 4.20]. Not pre-registered.

**Note 38.**

> Not all did: elementary school teachers, the third largest, were flat, and receptionists fell 3.4% a year.

BLS, Occupational Employment and Wage Statistics (OEWS), national May tables, via Wayback Machine copies of bls.gov, e.g. https://web.archive.org/web/20260516122846id_/https://www.bls.gov/oes/special-requests/oesm25nat.zip (May 2025) and https://web.archive.org/web/20240522032635id_/https://www.bls.gov/oes/2022/may/oes_nat.htm (May 2022); full list in analysis/data/part3/t1_t6/SOURCES.md and analysis/data/part3/t4_t5/SOURCES.md; our calculation (research_notes/part3-occupations.md, T5): annual growth May 2022 to May 2025; analysis/results_part3_t4_t5.json, T5 top_fifth_largest (the twelve largest top-fifth occupations by 2022 employment): home health and personal care aides +7.1, registered nurses +3.2, elementary school teachers -0.1 (third largest), nursing assistants +3.4, teaching assistants +4.2, security guards +4.5, secondary school teachers +0.7, receptionists and information clerks -3.4 (% a year).

**Note 39.**

> An ageing population, the growth of home care paid for by Medicaid, pandemic relief money for schools and immigration into care work all fit the pattern, and none of them is AI.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T5, point 3: the top fifth is about 74% (of 2022 employment; analysis/part3/redteam/rt_t4_t5.json, top_fifth_emp_share_by_major_group: SOC groups 21, 25, 29, 31 and 33) health care, education, social services and protective service; plausible drivers named (ageing, Medicaid home-care growth, pandemic relief money for schools, immigration into care work). Candidates only; not measured. Not part of the original plan (not pre-registered).

**Note 40.**

> Allowing for each occupation's 2019-2022 growth left it at 2.5.

Our pre-registration, "Pre-registration: the book's own tests (Part 3)", analysis/PREREGISTRATION.md (commit 93726bb, 22 October 2026, written before any of the tests was run and before most of their data were downloaded; the OEWS tables had been cached earlier for other chapters, and the T4/T5 files were downloaded before every detail was fixed), deviations of 2026-10-22 for T4 and T5 ("fixed before any employment growth was computed"): May 2022 estimates pool survey panels from November 2019 to May 2022; a 2019-2025 window and a control for 2019-2022 growth were declared there as labelled checks, not pre-registered. Results in analysis/results_part3_t4_t5.json, T5 sensitivity: window_2019_2025, most minus least person-facing +1.53 pp a year [0.16, 2.93] against +1.34 in 2016-2019 (difference +0.18 [-1.22, 1.58]); controlled_for_2019_2022_growth, +2.50 log points a year [1.39, 3.65] (uncontrolled +2.54). Both flagged pre_registered: false. research_notes/part3-occupations.md, caveat 1.

**Note 41.**

> As late as 2022 the American industry stood 2.4% above its line, and our planned comparison from before AI showed a shortfall of 2.8%, over a much shorter stretch.

BLS CES6054150001 (computer systems design and related services, NAICS 5415), https://data.bls.gov/timeseries/CES6054150001?from_year=2010&to_year=2026&output_view=data&include_graphs=false. Our calculation, analysis/results_part3_t1_t6.json: 2,370.8k against trend 2,654.2k, -10.7% [-11.6, -9.7]; planned pre-AI comparison -2.8% [-3.7, -1.8] (2017-19 gap from a 2012-16 line); 2022 gap +2.4% (exploratory); about -5% since December 2022 (Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T6). The 2022 gap was added after the results were seen; the red-team checks were not part of the original plan.

**Note 42.**

> One of the four, HCLTech, reached a new high in September 2026, after the dip in the June quarter that chapter 7 noted.

Firms' own reports: TCS and Infosys via Wayback Machine copies of their fact sheets (their sites block scripts); Wipro and HCLTech from wipro.com and hcltech.com. Four firms: 961,798 (March 2019), 1,440,894 (March 2023, +49.8%), 1,388,793 (June 2026, -3.6%); FY2022 +243,258; HCLTech 230,339 (September 2026). Infosys September 2026 not found. Wipro figures as first reported. June 2026 sources: TCS Q1 FY27 fact sheet, https://web.archive.org/web/20260828130818id_/https://www.tcs.com/content/dam/tcs/investor-relations/financial-statements/2026-27/q1/Presentations/Q1%202026-27%20Fact%20Sheet.pdf; Infosys Q1 FY27 fact sheet, https://web.archive.org/web/20260828130817id_/https://www.infosys.com/investors/reports-filings/quarterly-results/2026-2027/q1/documents/fact-sheet.pdf; Wipro Q1 FY27 data sheet, https://www.wipro.com/content/dam/nexus/en/investor/quarterly-results/2026-2027/q1fy27/datasheet-q1fy27.pdf; HCLTech Q1 FY27 investor release, https://www.hcltech.com/sites/default/files/documents/investor-reports/HCLTech_Q1_FY27_Investor_Release.pdf. September 2026: HCLTech Q2 FY27 investor release, https://www.hcltech.com/sites/default/files/document/open/quarter-results/2026-10/hcltech-Q2-fy27-Investor-release.pdf (all retrieved 2026-10-22). URLs for each fact sheet and release, with Wayback copies, are listed in analysis/data/part3/t1_t6/raw/web/headcount_urls.csv and analysis/data/part3/t1_t6/it_headcounts.csv.

**Note 43.**

> The red team found that before AI a straight line carried this far ahead missed by at least as much in 15 of 19 periods, counting misses in either direction; 6 of the 19 had a shortfall this large.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T6: at the same horizon, 15 of 19 pre-AI windows missed by at least 10.7 points in absolute terms; 6 of 19 had a shortfall at least this large. Not pre-registered. The red team drops the earlier "3.9 times its placebo" comparison.

**Note 44.**

> The industry body Nasscom estimated, in February 2026, that direct Indian technology employment would reach about 6 million for the 2026 financial year, up 2.3%, so the industry as a whole kept adding people while its four largest firms shrank from their peak.

Nasscom, Strategic Review 2026, Executive Summary, February 2026: estimate published February 2026: Indian direct tech employment about 6 million in FY26E (the 2026 financial year), up 2.3%, net addition 135,000. https://nasscom.in/modules/custom/nasscom_general/docs/Nasscom-Strategic%20Review-2026-Executive%20Summary.pdf (retrieved 2026-10-22).

## Chapter 14: What the Data Say So Far, and How to Keep Score

**Note 1.**

> Over the same three years, market research analysts grew by about 4.0% a year, management analysts by 3.6% and human resources specialists by 3.0%.

Our calculation, analysis/part3/t4_t5/analyse.py, results in analysis/results_part3_t4_t5.json (OEWS May 2022 and May 2025 national estimates, BLS, Wayback copies of https://www.bls.gov/oes/special-requests/oesm22nat.zip and oesm25nat.zip; exposure scores from Eloundou et al., 2023). Annualised growth May 2022 to May 2025: customer service representatives -3.4%, receptionists -3.4%, secretaries -2.2%, office clerks -0.7%; market research analysts +4.0%, management analysts +3.6%, HR specialists +3.0%. All in the most-exposed fifth. Research note: research_notes/part3-occupations.md §1, T4.

**Note 2.**

> As with the routes in chapter 13, what would count against the book was written down before any growth rate was computed.

Our pre-registration, analysis/PREREGISTRATION.md, T4, written 22 October 2026 before any outcome data for these tests was downloaded (commit 93726bb, 06:51 Pacific time); implementation details in its Deviations entry "T4 and T5" (dated 2026-10-22), fixed before any employment growth rate was computed (it discloses that files were downloaded and their layouts inspected first); results committed at 07:13 the same morning (commit a1e8af5). Chapter 13 explains the general method (pre-registration, before-AI comparison, intervals, red team).

**Note 3.**

> Their scores capture what AI could do, as rated in 2023, and do not show whether anyone has put it to use.

Eloundou, Manning, Mishkin and Rock, "GPTs are GPTs: An Early Look at the Labor Market Impact Potential of Large Language Models", arXiv:2303.10130 (v5, August 2023), https://arxiv.org/abs/2303.10130; published in *Science* 384(6702), 2024. Score used: human-rated beta (E1 + 0.5·E2), data MIT licence. The authors state they make no predictions about adoption timelines. Research notes: economics.md (Eloundou entry); part3-occupations.md §4.4.

**Note 4.**

> We ranked the units into five equal groups by exposure, then compared how fast jobs grew in the most exposed fifth and the least exposed fifth.

Our calculation, analysis/part3/t4_t5 (build_data.py, analyse.py). OEWS May 2016 (SOC 2010), May 2019 (OES hybrid codes), May 2022 and May 2025 (SOC 2018), joined through the BLS SOC 2010-2018 crosswalk and the OES 2019 hybrid list into 775 harmonised units with employment in all four years (99.96% or more of employment kept each year); 762 scored for exposure. Sources and hashes in analysis/data/part3/t4_t5/SOURCES.md. Research note: part3-occupations.md, method paragraph.

**Note 5.**

> The test carries the two safeguards chapter 13 described: the same test run on May 2016 to May 2019, as the fair comparison from before AI, and a range for every result, reported whatever it shows.

Method explained in chapter 13. Our pre-registration, analysis/PREREGISTRATION.md (commit 93726bb, written 22 October 2026 before outcome data), ground rules (placebo 2016-2019; 95% bootstrap intervals, 10,000 resamples, seed 20261022; results reported whatever they show) and T4; bootstrap over units within each fifth per the Deviations entry "T4 and T5".

**Note 6.**

> Before ChatGPT the same gap was almost exactly zero (+0.02).

Our calculation, analysis/results_part3_t4_t5.json, T4. Least-exposed fifth (153 units, 19.1m jobs in 2022) +0.67% a year [-0.08, 1.40]; most-exposed fifth (152 units, 37.1m jobs) +1.12% [-0.14, 2.30]; difference +0.45 percentage points a year [-0.97, +1.87]; placebo May 2016 to May 2019 +0.02 [-1.70, 1.85]. Chart: analysis/part3/t4_t5/charts/t4_exposure_fifths.png. Research note: part3-occupations.md §1.

**Note 7.**

> The range runs about one and a half points either side, and over three years that leaves room for roughly 4% to 5% of employment to move one way or the other without the test seeing it.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T4, safe sentence (exposure) and caveat on power: an interval of about ±1.5 points a year over three years means about 4-5% of employment could move either way unseen. Not pre-registered.

**Note 8.**

> The one version whose range sat clear of zero, a window from 2019 that we had not planned, showed exposed jobs within the same family growing faster.

> That one deserves attention, because a later and shorter window is where an early effect would first appear.

> The survey reports employers' payrolls by occupation, pooled across all ages, and builds each May figure from three years of survey rounds, so "2022 to 2025" compares, roughly, 2021 with 2024, and May 2023 still holds rounds from before ChatGPT.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T4 checks and results table (rt_t4_t5.json): leave-one-out of the 10 largest units +0.14 to +0.81; unweighted median +0.52; continuous score per SD -0.26 [-0.86, 0.35]; controlling for 2016-19 growth -0.28; within SOC major groups +0.29 [-0.49, 1.14], and over 2019-25 +0.80 [0.22, 1.43]; May 2023 to May 2025 on SOC 2018 codes -0.23 [-1.70, 1.29]. From the research note's sensitivity table (research_notes/part3-occupations.md): GPT-4-rated beta -0.43 [-1.90, 0.97], against -0.84 before ChatGPT (difference +0.14 [-1.50, 1.99]); controlled for 2019-22 growth -0.46 log points [-1.98, 0.98]. The continuous and growth-controlled rows are per standard deviation of exposure; the GPT-4 row is a top-minus-bottom gap in points a year. Caveats: OEWS May estimates pool three years of survey panels (so 2022 to 2025 compares roughly 2021 with 2024; May 2023 still contains pre-ChatGPT panels), and all ages are pooled. Not pre-registered.

**Note 9.**

> Pooling hides the group hit hardest so far, which chapter 5 described: workers aged 22 to 25 in exposed jobs, whose numbers in payroll data have fallen well behind those of their less exposed peers.

Brynjolfsson, Chandar and Chen, "Canaries in the Coal Mine? Six Facts about the Recent Employment Effects of Artificial Intelligence", Stanford Digital Economy Lab, 2025, revised August 2026 (ADP payroll data to June 2026), https://digitaleconomy.stanford.edu/app/uploads/2026/08/Canaries_August2026.pdf. Employment of 22-25-year-olds in AI-exposed occupations stands 19% below where it would be had it kept pace with less exposed peers. Chapter 5 reports this in full. Research note: part3-occupations.md §3; red team T4 caveats.

**Note 10.**

> We matched those conversations to occupations and split the 282 units in the two most exposed fifths that had any usage data at the middle.

Anthropic Economic Index, release 2025-03-27 (automation_vs_augmentation_by_task.csv and task_pct_v2.csv, Hugging Face commit 4e5f69f), https://huggingface.co/datasets/Anthropic/EconomicIndex; Handa et al., "Which Economic Tasks are Performed with AI? Evidence from Millions of Claude Conversations", arXiv:2503.04761, 2025. Augmentation = validation + task iteration + learning; automation = directive + feedback loop. Of the 304 units in the two most exposed fifths, 282 had usage data (22 without, 2.3m jobs); split at the median augmentation share, 0.635. Our matching: analysis/part3/t4_t5; PREREGISTRATION Deviations "T4 and T5".

**Note 11.**

> Before ChatGPT, the same two halves were already about 0.91 points apart in the same direction.

Our calculation, analysis/results_part3_t4_t5.json, T4 augmentation split: more-automated half +1.85% a year [0.81, 2.89], more-augmented half +0.80% [-0.34, 2.15]; difference -1.05 pp [-2.60, +0.68]; placebo 2016-19 -0.91 [-2.62, 1.03]. Wording follows the red team safe sentence (augmentation). Chart: analysis/part3/t4_t5/charts/t4_augmentation_split.png.

**Note 12.**

> Leave those three out and the gap falls to about a quarter of a point.

> The red team found that it stops being clear once those same three occupations are removed, and this chapter drops the claim.

> At best it describes how people phrase requests to a chatbot, which may be far from how their employers have set up the work.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T4 augmentation split: without retail salespersons, cashiers and customer service reps -0.27 (placebo -0.52); the 2019-25 window, -2.43 [-4.05, -0.28] in the research note (part3-occupations.md, which called it "clearly negative"), becomes -1.41 [-3.21, 0.71] without the three; measure weaknesses (one company's users, early 2025, after the outcome window, median summed task share 0.09, describes phrasing of requests). AEI shares: retail salespersons 0.77, cashiers 0.77, customer service reps 0.68. Not pre-registered.

**Note 13.**

> The one real limit it sets is on this book: we cannot cite our own occupation data as evidence that augmenting protects jobs.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, "Does T4 contradict chapter 9?"; chapter 9 of this book, section "The missing trial".

**Note 14.**

> That last is a difference our own split could not detect, and it leans the book's way; the two can both hold, since they count different workers with a different measure.

> If that gap spreads to experienced workers, the first forecast above is in trouble.

Brynjolfsson, Chandar and Chen, "Canaries in the Coal Mine?", Stanford Digital Economy Lab, revised August 2026, https://digitaleconomy.stanford.edu/app/uploads/2026/08/Canaries_August2026.pdf. They report "no evidence of widespread, economy-wide job displacement"; the young-worker gap with no comparable gap for experienced workers; declines concentrated where AI automates rather than complements. Research note: part3-occupations.md §3 [V].

**Note 15.**

> The Danish study from chapters 1 and 5 rules out chatbot effects bigger than 2% on earnings or recorded hours two years after ChatGPT.

Humlum and Vestergaard, "Still Waters, Rapid Currents: Early Labor Market Transformation under Generative AI", NBER Working Paper 33777, May 2025, revised March 2026, https://www.nber.org/system/files/working_papers/w33777/w33777.pdf (abstract; abstract page https://www.nber.org/papers/w33777): Denmark, adoption surveys linked to administrative records; "precise null effects on earnings and recorded hours", "ruling out effects larger than 2% two years after the launch of ChatGPT"; tasks reorganised within jobs. Research note: part3-occupations.md §3.

**Note 16.**

> And the Budget Lab at Yale, in the report chapter 11 quoted, found that measures of exposure, automation and augmentation show "no sign of being related to changes in employment or unemployment."

Gimbel, Kinder, Kendall and Lee, "Evaluating the Impact of AI on the Labor Market: Current State of Affairs", The Budget Lab at Yale, 1 October 2025, https://budgetlab.yale.edu/research/evaluating-impact-ai-labor-market-current-state-affairs. Key takeaways: the occupational mix is changing somewhat faster than in the past, a change that "predates the widespread introduction of AI"; "measures of exposure, automation, and augmentation show no sign of being related to changes in employment or unemployment." Later updates were seen only in search summaries and are not used. Research note: part3-occupations.md §3.

**Note 17.**

> Sources for the table are in the note.

> The build-out can't be called yet: only power utilities clearly turned up after 2022, and gas utilities rose with them.

Our calculations: analysis/results_part3_t1_t6.json (T1, T6), analysis/results_part3_t2_t3.json (T2, T3), analysis/results_part3_t4_t5.json (T4, T5); research notes part3-buildout-research-it.md, part3-newfirms-spending.md, part3-occupations.md. Verdicts and wording from Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, summary of verdicts and safe sentences: T1 weaker than reported in both directions (same-horizon pre-AI misses of 26-58 points for three series and 8.7 for power utilities; gas distribution +11.8%); T2 primary holds (fragile), secondary a 2025-26 model projection; T3-A holds as computed, break-even reading; T3-B holds with caveat (Baumol); T4 holds with caveat; augmentation split uninformative; T5 formal fail holds as a near miss, gap real but not tied to AI; T6 descriptive. Verdict labels in the table are the chapter's condensation of the red team's: T1 "No call yet" (none of the five series counts for or against the book; power utilities the one series that clearly turned up after 2022, +8.9% since December 2022, with gas utilities rising too); T3-A against the book as planned, with the spending-weighted slope (+0.25 [0.02, 0.68], not planned) in Hypothesis A's direction; T4 augmentation "Not supported" (no advantage, no clear disadvantage; the red team calls the split uninformative); T6 description only (cannot separate AI from interest rates and the end of pandemic hiring).

**Note 18.**

> Only one result survives: T3-B, the finding that jobs followed spending.

> That spending went mostly into services that were getting dearer, such as health care and education, so this shows jobs following spending, not spending freed by things getting cheaper.

Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, "Multiple comparisons (Holm, α = 0.05)" (rt_holm.json): with the book's own benchmarks five of 11 contrasts survive, but the T1 p-values rest on line-only intervals; replaced by same-horizon rank p-values (smallest possible 0.05 with 19 windows), only T3-B survives (p = 0.0025 < 0.05/10). The family has ten comparisons: four T1 series (2211, 518, 23713, 3344; electricians left out because all their same-horizon windows fall in the housing bust), T2, T3-A, T3-B, T4 exposure, T4 augmentation and T5. Holm tests the smallest p-value at 0.05/10, the next at 0.05/9, and so on, and stops at the first that fails. Holm guards against false positives only. T3-B interpretation: gainers got relatively dearer (health care +0.27 log, education +0.94). Not pre-registered.

**Note 19.**

> The tests and their "against the book" rules were planned before the results; what came after, the red team's review included, is marked as unplanned in the notes.

Our pre-registration, analysis/PREREGISTRATION.md (commit 93726bb, written 22 October 2026 before outcome data), Deviations, entries of 22 October 2026, including "T1 and T6, additions made after the results were seen" (2022 gaps; forecast method and widening; T4 without the three large merged units; augmentation split on above-median usage; group forecast as shares). The red-team review states that everything in it is not pre-registered.

**Note 20.**

> Each one below is this book's own, carried forward from the data named with it, with a range and the observation that would prove it wrong.

Our pre-registration, analysis/PREREGISTRATION.md (commit 93726bb, written 22 October 2026 before outcome data), section "Forecasts" (range, assumptions, falsifier) and the Deviations entry on the forecast method: Jan 2023-latest straight line continued to 2028, range the wider of a 12-month block bootstrap and the 2.5-97.5 percentiles of the method's pre-2020 back-test errors (24 forecasts; -3.78% to +7.36%), chosen after the data were seen; the ranges were widened the same day to match how far the same method missed before 2020.

**Note 21.**

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4%

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years | Same | Gap 1 to 4 points a year; growth 13% to 25% | Missed if the gap is outside 1 to 4 points; wrong in direction if it is zero or below | | Office work's share of jobs, May 2030: office and administrative support falls from 11.4%; healthcare support rises from 5.1%

Our projection, analysis/results_part3_t4_t5.json, "forecasts" (T4_exposure_fifths_to_2030, T5_person_fifths_to_2030, major_groups_share_to_2030), dated 22 October 2026, OEWS data to May 2025. Exposure: most-exposed fifth +5.7% over 2025-2030 [-0.7, +12.1], least-exposed +3.4% [-0.4, +7.2]; falsifier a shortfall over 1.5 pp a year. Person-facing: +19.2% [13.3, 25.2]; gap +1 to +4 pp a year. Shares: office and administrative support 11.42% (2025) to 9.65-10.21% (2030); healthcare support 5.08% to 6.01-6.20%. Group shares method added after the results (Deviations); its range spans each group's 2016-19 and 2022-25 growth relative to all jobs. Falsifiers: "missed" outside the range; "wrong in direction" at or beyond the 2025 level (office at or above 11.4%, healthcare support at or below 5.1%; person-facing gap at or below zero). Research note: part3-occupations.md §2.

**Note 22.**

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years | Same | Gap 1 to 4 points a year; growth 13% to 25% | Missed if the gap is outside 1 to 4 points; wrong in direction if it is zero or below | | Office work's share of jobs, May 2030: office and administrative support falls from 11.4%; healthcare support rises from 5.1% | Same | Office 9.7% to 10.2%; healthcare 6.0% to 6.2% | Missed if either share is outside its range; wrong in direction if office is at or above 11.4%, or healthcare at or below 5.1% | | Power utility jobs, 2028 average: about 448,000, above the 2015-2019 trend line of about 371,000

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years | Same | Gap 1 to 4 points a year; growth 13% to 25% | Missed if the gap is outside 1 to 4 points; wrong in direction if it is zero or below | | Office work's share of jobs, May 2030: office and administrative support falls from 11.4%; healthcare support rises from 5.1% | Same | Office 9.7% to 10.2%; healthcare 6.0% to 6.2% | Missed if either share is outside its range; wrong in direction if office is at or above 11.4%, or healthcare at or below 5.1% | | Power utility jobs, 2028 average: about 448,000, above the 2015-2019 trend line of about 371,000 | Payroll survey, August 2026 | 431,000 to 481,000 | At or below 371,000, or outside the range | | IT services jobs, 2028: computer systems design about 2.29 million, below its old trend line of about 2.81 million

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years | Same | Gap 1 to 4 points a year; growth 13% to 25% | Missed if the gap is outside 1 to 4 points; wrong in direction if it is zero or below | | Office work's share of jobs, May 2030: office and administrative support falls from 11.4%; healthcare support rises from 5.1% | Same | Office 9.7% to 10.2%; healthcare 6.0% to 6.2% | Missed if either share is outside its range; wrong in direction if office is at or above 11.4%, or healthcare at or below 5.1% | | Power utility jobs, 2028 average: about 448,000, above the 2015-2019 trend line of about 371,000 | Payroll survey, August 2026 | 431,000 to 481,000 | At or below 371,000, or outside the range | | IT services jobs, 2028: computer systems design about 2.29 million, below its old trend line of about 2.81 million | Payroll survey, September 2026 | 2.21 to 2.46 million | At or above 2.81 million, or outside the range | | Data processing and hosting, 2028: about 453,000, on the old trend line, no call on direction

Our projection, analysis/results_part3_t1_t6.json, forecasts_2028, dated 22 October 2026: BLS CES (data.bls.gov series pages) through September 2026 (August 2026 for power utilities, CES4422110001). Power utilities 448k [431, 481], 2015-19 trend line 371k; computer systems design (CES6054150001) 2,293k [2,207, 2,462], trend line 2,808k; data processing and hosting (CES5051800001) 453k [436, 487], trend line 453k, no directional call. Assumptions: the Jan 2023-latest straight line continues, no recession, no NAICS change. T6 caveats from Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, T6 safe sentence. The pre-registration ("Forecasts") used data processing as its example of a forecast (that it stays above trend); the data no longer point that way, since employment has fallen since 2023 (-6.6% since December 2022, red team T1). Research note: part3-buildout-research-it.md §2.

**Note 23.**

> | Forecast | Data to | Range | Wrong if | |---|---|---|---| | Exposure and jobs, May 2025 to May 2030: at 2022-2025 rates, the most exposed fifth grows about 5.7% over five years and the least exposed 3.4% | Occupation survey, May 2025 | Most exposed -0.7% to +12.1%; least exposed -0.4% to +7.2% | The most exposed fifth grows more than 1.5 points a year more slowly than the least | | Person-facing work, to May 2030: the most person-facing fifth outgrows the least and grows about 19% in five years | Same | Gap 1 to 4 points a year; growth 13% to 25% | Missed if the gap is outside 1 to 4 points; wrong in direction if it is zero or below | | Office work's share of jobs, May 2030: office and administrative support falls from 11.4%; healthcare support rises from 5.1% | Same | Office 9.7% to 10.2%; healthcare 6.0% to 6.2% | Missed if either share is outside its range; wrong in direction if office is at or above 11.4%, or healthcare at or below 5.1% | | Power utility jobs, 2028 average: about 448,000, above the 2015-2019 trend line of about 371,000 | Payroll survey, August 2026 | 431,000 to 481,000 | At or below 371,000, or outside the range | | IT services jobs, 2028: computer systems design about 2.29 million, below its old trend line of about 2.81 million | Payroll survey, September 2026 | 2.21 to 2.46 million | At or above 2.81 million, or outside the range | | Data processing and hosting, 2028: about 453,000, on the old trend line, no call on direction | Same | 436,000 to 487,000 | Below 436,000 or above 487,000 | | Professional services such as legal and accounting, 2030: if AI cuts their relative price by 25%, their share of consumer spending, 1.446% ($302 billion) in 2025, stays within the range

Our projection, analysis/results_part3_t2_t3.json, T3 projection: BEA NIPA Table 2.4.5 line 104 "Professional and other services", 1.446% of PCE ($301.9bn) in 2025; relative price cut 25%: share 1.303-1.600%; 40%: freed spending -$59.2bn to +$51.2bn (negative = more spending on the category), central -$2.7bn. NIPA Tables 2.4.4 and 2.4.5 from BEA's release text files, https://apps.bea.gov/national/Release/TXT/. Spending-weighted slope (+0.25) and trimmed slope (+0.22) give $36bn and $32bn freed at a 40% cut: Our red-team review, "Red team: the six pre-registered tests (T1-T6)", 22 October 2026, analysis/part3/redteam/REDTEAM.md, "T3 projection" (not pre-registered). Falsifier: a relative price fall of about a quarter (20% to 30%) by 2030 with the share outside 1.30-1.60% (the 25% range; 1.20-1.73% is the 40% range). Research note: part3-newfirms-spending.md §2.

**Note 24.**

> For productivity, Acemoglu, as chapter 5 reported, estimated in 2024 that AI would add no more than 0.66% to total factor productivity over ten years in all; the OECD's economists put AI's addition to American total factor productivity growth at 0.25 to 0.6 of a percentage point every year for a decade; and the Penn Wharton Budget Model expects AI to leave productivity and GDP 1.5% higher by 2035.

D. Acemoglu, "The Simple Macroeconomics of AI", NBER Working Paper 32487, May 2024 (ten-year total), https://www.nber.org/system/files/working_papers/w32487/w32487.pdf; F. Filippucci, P. Gal and M. Schief, "Miracle or Myth? Assessing the macroeconomic productivity gains from Artificial Intelligence", OECD Artificial Intelligence Papers No. 29, November 2024, as summarised on the OECD ECOSCOPE blog, 26 November 2024 (per year, US TFP), https://oecdecoscope.blog/2024/11/26/miracle-or-myth-assessing-the-macroeconomic-productivity-gains-from-artificial-intelligence/; Penn Wharton Budget Model, "The Projected Impact of Generative AI on Future Productivity Growth", 8 September 2025, https://budgetmodel.wharton.upenn.edu/p/2025-09-08-the-projected-impact-of-generative-ai-on-future-productivity-growth/. Moved from chapter 12 (its former notes 29-31).

**Note 25.**

> These are employers' expectations.

World Economic Forum, *Future of Jobs Report 2025*, January 2025 (employer survey, 2025 to 2030), https://reports.weforum.org/docs/WEF_Future_of_Jobs_Report_2025.pdf. Employers' expectations. Same survey: "40% planning to reduce staff as their skills become less relevant, and 50% planning to transition staff from declining to growing roles" (claims.md 12.43 / 14.40; whole-book fix W3). Moved from chapter 12 (former note 32).

**Note 26.**

> The IMF warned in January 2026 that the spread of demand for AI skills goes with lower employment in jobs where AI can do much of the work and helps little with the rest, a challenge for young workers that may shrink the middle class.

Jaumotte, Kim, Koll, E. Li, L. Li, Melina, Song and Tavares, "Bridging Skill Gaps for the Future: New Jobs Creation in the AI Age", IMF Staff Discussion Note, 14 January 2026, https://www.imf.org/en/Publications/Staff-Discussion-Notes/Issues/2026/01/09/Bridging-Skill-Gaps-for-the-Future-New-Jobs-Creation-in-the-AI-Age-572136. Summary page read; the full text was not. Moved from chapter 12 (former note 33).

**Note 27.**

> The exact series codes are in the note.

Series codes: BLS CES4422110001 (electric power generation, transmission and distribution) and CES6054150001 (computer systems design and related services); BLS OEWS May national estimates, major groups 43 (office and administrative support) and 31 (healthcare support); Census Business Formation Statistics BA_HBA and BF_PBF4Q, NAICS sectors 54 and 51; BEA NIPA Tables 2.4.4 (prices) and 2.4.5 (spending), line 104 "Professional and other services"; Census Construction Spending, private, "Data center". Chapter 13 gives the latest data-centre figure: US Census Bureau, Construction Spending (C30), private construction, seasonally adjusted annual rate, "Data center", release of 1 October 2026: $84.95bn (August 2026, preliminary) against $8.8bn (August 2019), https://www.census.gov/construction/c30/xlsx/privsatime.xlsx, retrieved 2026-10-22. Research note: part3-buildout-research-it.md §3.1. Other watch-list series: BLS CES CES4422110001 and CES6054150001 (https://data.bls.gov/timeseries/); BLS OEWS May national estimates (https://www.bls.gov/oes/2025/may/oes_nat.htm pattern; our copies via the Wayback Machine, analysis/data/part3/t4_t5/SOURCES.md); Census Business Formation Statistics BA_HBA and BF_PBF4Q (https://www.census.gov/econ/bfs/csv/bfs_monthly.csv); BEA NIPA Tables 2.4.4 and 2.4.5 (https://apps.bea.gov/national/Release/TXT/). BLS cautions that OEWS is designed for cross-sectional comparison (part3-buildout-research-it.md §4).

