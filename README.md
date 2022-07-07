# Belly_Button_Biodiversity

Link for interactive dashboard: https://jwetapatel.github.io/Belly_Button_Biodiversity/

# Overview of Project

Rosa needs to visualize and creat a Dashboard of the bacterial data for each volunteer. Specifically, her volunteers should be able to identify the top 10 bacterial species in their belly buttons. That way, if Improbable Beef identifies a species as a candidate to manufacture synthetic beef, Roza's volunteers will be able to identify whether that species is found in their navel.

# Resources

D3, Plotly, Bootstrap, Javascript, Html, VS Code

# Results


1. Drop down and Demographics panel: The first step was to add all the IDs to the “Test Subject ID No” dropdown so that the user can select which ID they would like to look at and so we can use that ID to parse out the information that we need from our data json file. I then use the ID to filter out the metadata pertaining to the selected ID and stored it in an object. I then used d3 to select the panel-body class in my index.html where I used a forEach statement to iterate through the object and append the data to the demographics panel.

![id_image](https://user-images.githubusercontent.com/96400887/177813193-2ac87ac7-818b-4c92-897a-99ad39368848.png)

2. Horizontal bar chart and Bubble Chart: To create the horizontal chart, I first filtered the JSON data by the current ID that the user has selected. I then created a trace for the chart with the top 10 sample values as the x and the OTU IDs as the y. I then used Plotly to create the bar chart. I followed the same steps above to create the bubble chart.

![Bar graph](https://user-images.githubusercontent.com/96400887/177814071-685301b2-cbb0-49bb-b109-faa482bf4d49.png)

![bubble chart](https://user-images.githubusercontent.com/96400887/177814074-648b7cdb-65bb-405e-ba3e-4394b4c28ef1.png)

