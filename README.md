# Upland-Capstone
Real Estate Metaverse R Programming Analysis


This is my Capstone Project for the Merit America bootcamp program. 
Please download all files as they are referenced in the R notebook Notebook.Rmd
You may experience compatibility issues working with different platforms. 

This analysis uses data from Upland, a metaverse property trading game. You can find more information about it at http://upland.me. I used the data from my own portfolio.
My main goals of the analysis was to use R to show which cities and neighborhoods have the highest land value, which of my purchases were the least profitable, and which neighborhoods and cities had the highest ROI. 
The game follows certain rules, but we are treating the project as if it is a mock real estate company and we are making suggestions to stakeholders. Therefore, some of the recommended actions will try to incorporate real world economic conditions.

I began by loading several packages that I would use in the analysis.
First, I wanted to test for the internal validity of the data. I began with a sample of 10,199 of Upland's San Francisco Properties.
Data cleaning was a simple process. The game uses a consistent pricing scheme for currency yeld per square foot for each neighborhood, so I sorted my properties by neighborhood.
I discovered 2 glitched properties and 28 properties with a null neighborhood field because they were on the border of two neighborhoods. These entries were eliminated from the dataframe. 
Once that was complete, I created a chart of neighborhood rents and they were all consistent. I was ready to begin the analysis of my own portfolio.

I exported my portfolio of 544 properties and put it into a dataframe. 
Naturally I had to check for the clenliness of this data the same way, but found no null or erroneous entries. 

Question 1: Which cities and neighborhoods have the highest land value?
I created two charts showing the highest land values by city and by neighborhood.
London was found to be the most expensive while Fresno and Bakersfield were found to be the least expensive. This came as no surprise because the game is designed this way.
London is meant to be a more exclusive city while Fresno and Bakersfield are more affordable for new or younger players. 

Question 2: Which of my purchases were the least profitable?
Upland properties are sold at what is called mint value when there is no previous owner and a player is purchasing the property for the first time. Players then try to trade or sell those properties for a higher price later on. 
Therefore, the most profitable purchases will be those you are getting at mint price. My findings reflected this and there were no surprises. 
I decided that 32 of my properties were bad buys because I purchased them at too high of a price. 

Question 3: Which neighborhoods and cities have the highest ROI?
This is similar to our first question. The main difference is that we are looking to calculate using the paid price rather than the mint price for each property.
This will reflect my own ROI in each community rather than the land value.
As expected, my best ROI comes from communities where I made the most mint purchases. 

After answering these questions I created visualizations to communicate my findings. 
I created charts for land value by city, differences in marked up vs mint purchase prices, and ROI by city. 
I also created ROI Charts for neighborhoods within a few cities. 

Recommendations to Stakeholders:
Focus on acquiring more properties in London - these are high yield properties with a high entry price so there is more reward and less competition.
Avoid buying new properties at a markup. Focus only on minting new properties. 
Develop properties that have been lower ROI with virtual structures to make them more appealing and raise potential resale value. Alternatively, consider selling them to get funds for properties in better locations.
