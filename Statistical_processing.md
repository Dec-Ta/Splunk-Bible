Transforming Data
Data Series:
Single Series
A sequence of related data points that compares values of a single
data category

Multi-Series
A sequence of related data points that compares values of two or
more data categories 

Time-Series
A (single or multi-series) sequence of related data points that compares values over time

Chart
index=security sourcetype=linux_secure
| chart count by vendor_action user

index=security sourcetype=linux_secure
| chart count by vendor_action user useother=f

span
used if the x-axis is numeric
example:
index=indexname sourcetype=sourcetype_name
| chart span=100 count over status by host

limit

useother
useother=f (do not include "other" category
usenulll=f (do not include null values

TImechart

example:
| timechart <stats-func>(<field>) by <split-by-field>
[span=<int><timescale>] [limit=<int>]

Top
Rare

Manipulating Data
-Eval
--pow
--round
--min
--max
--random

Formatting Data
-Rename
-Sort
