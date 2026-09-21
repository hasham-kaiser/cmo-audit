# CMO Marketing Audit

A marketing audit of six campaigns across 2,229 retail customers, identifying where 
campaign effort pays off, where it is wasted, and what to change.

**[View the full notebook →](cmo-audit.ipynb)**

## Verdict

Most campaign results come from one campaign and one type of customer: high income 
customers in small households. Campaign 2, and catalogs sent to low income and large 
households, deliver almost nothing.

## Key Findings

- **Campaign performance splits sharply.** The final campaign converted at 14.8%, twice 
the 7.4% average. Campaign 2 converted at 1.3%, roughly six times below it.
- **Conversion concentrates in high income, small households.** High income customers 
convert at 48.4% against 14.2% for low income. Single customers convert at 50.8% 
against 12.5% for the largest households. Age shows almost no effect.
- **Wines and meat drive revenue and separate responders from non-responders.** They 
make up 77% of average spend, and responders outspend non-responders by 2.5x on wines 
and 2.2x on meat, against roughly 1.6x elsewhere.
- **Catalog only works for high income customers.** Catalog share rises from 8.7% of 
low income purchases to 29.5% of high income purchases, and falls from 28% to 13% as 
household size grows.

## Recommendation

| Cut | Hold | Double |
|---|---|---|
| Campaign 2 | Campaigns 1, 3, 4, 5 | The final campaign's approach |
| Catalogs to low income and large households | | High income, one or two person households |
| | | Wine and meat led offers |
| | | Web for large families |

## Approach

1. **Cleaning.** Dropped constant columns, filled missing income with the median, 
removed impossible birth years, an extreme income outlier and invalid marital status 
entries (2,240 to 2,229 records).
2. **Feature engineering.** Built total spend, campaigns accepted, age, tenure, family 
size, a responder flag, and income and age segments.
3. **Analysis.** Answered four audit questions on campaigns, segments, products and 
channels, each with one chart and a headline finding.
4. **Recommendation.** Synthesised the findings into a cut, hold and double reallocation.

## Tools

Python, pandas, matplotlib, seaborn, Kaggle Notebooks

**Data:** [Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis), Kaggle
