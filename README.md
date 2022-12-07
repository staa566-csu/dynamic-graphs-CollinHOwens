# dynamic-graphs-CollinHOwens
dynamic-graphs-CollinHOwens created by GitHub Classroom

This graph is a continuation of the last graph. This includes interactive options like choosing the item, choosing the date range of an update, and looking at prices in a time frame.

Questions from canvas.
Data source: From this website <https://www.lostarkmarket.online/north-america-west/market/enhancement-material> but I am using the API <https://documenter.getpostman.com/view/20821530/UyxbppKr> and used HTTR to automatically pull the data or else you can make an account through postman and download the data manually clicking in the top right of that second link. 

To recreate this, I would suggest installing the packages at the top because making an account is annoying along with downloading the CSV file. On the postman site, you would also have to specify the specific fields. If you wished to download the CSV, here are the fields you would fill out within the brackets in the paragraph following the note.

Note: if you changed regions the outliers would not be cleaned up due to my cleaning targetting very specific values that other regions would not have. Outside of outlier cleanup, the code can be applied for any region and the graphs would also be correctly displayed outside of the strange potential values.


{
region: North America West

items: basic-oreha-fusion-material-2,crystallized-destruction-stone-0,crystallized-guardian-stone-0,great-honor-leapstone-2,honor-shard-pouch-l-3,honor-shard-pouch-m-2,honor-shard-pouch-s-1,solar-blessing-2,solar-grace-1,solar-protection-3
}


What I want to convey: I want to show the prices of the items after certain events have been announced. The dates will be put at the bottom of the page, and the shaded regions will explain the announcement to application periods.

Functionality and formatting: The functionality I placed was the dynamic graphing that when you hover over a graph it shows the Y value and Date, and the left side will provide either a dropdown menu or buttons for enabling shaded regions. For both of these graphs I also added a rangefinder so you can look at specific dates or slide the bottom to cover a specific date range highlighted in the SuperLine graph. With a date variable and prices, time series was the most appropriate and Plotly had great options to help show the data.

  For the SuperLine graph, I added the shaded regions because on my final graph, the superline graph, 10 item's prices were added so that you can be compare them with each other. Due to plotly's option of clicking items to hide/see them, I was able to add buttons on the left side to highlight specific regions that cover certain dates. This was very useful because you can check different items and how the prices were affected due to the announcement and the application of the patch in the game.

  For the candlestick chart, I added a dropdown menu because there were large fluctuations in prices and having multiple candlestick charts stacked on top of eachother would make it very hard to read the graphs. Unfortunately I did not discover a way to highlight certain dates with this type of graph, but I believe with shiny apps/ Dashboards I can apply the candlestick chart dropdown and combine the graphs. Nonetheless, I do think it is a fun graph because if you see the SuperLine graph and see some major spikes, you could go to the candlestick graph and check the specific items highest and lowest prices of the day along with if the final price was lower than the previous day.
