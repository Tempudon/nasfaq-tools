# nasfaq-tools

## nasfaq-adjustment-predictor
Uses Python 3.6.9, optimized for Google Colab, based on TFT's Nasfaq helpers  
Queries HoloPoi API and Nasfaq to compare number of views gained each day  
Run after 0:00 UTC for results for following adjustment

Results are separated into Buy, Small Buy, Sell, Small Sell and are sorted by percent change from previous day. Green numbers indicate Holos that were forecasted to
have adjusted up the previous adjustment, while red indicates a forecasted adjustment down for the last adjustment. An asterisk indicates Holos that may be at risk of overbuy/oversell
based on their performance today vs two days ago. Also displays Holos that have gained 10k or more subs for the day.

Results table shows Holo name, percent difference from previous day, views gained today, views gained yesterday, views gained two days ago, and average views for the past week.

<b>Usage:</b>

Download .ipynb file and import into Google Colab  
Run all anytime after 0:00 UTC for results for following adjustment  
Check results in the tables at the bottom, make your own informed decisions based on the data, current trends (oversell/buy), and future streams/events  

<b>TO-DO:</b>

Fix issue where days with negative views don't display correct percent difference  
Create UI for results with ability to sort by different metrics  
Query nasfaq for more accurate statistics for whether a coin adjusted up or down the previous adjustment  
Integrating sub gains into results  
Allow script to be run at any point of the day, showing only Holos who have updated  
Clean up and move code to a consolidated Python file  
Future update: query Youtube API to Count views of videos from after Poi update cutoff to get buy/sell predictions as soon as possible at post-adjustment  
