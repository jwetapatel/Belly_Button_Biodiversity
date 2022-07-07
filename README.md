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

3. Gauge chart: To create the gauge chart, I first created my pie chart which would have the gradient colors and labels from lowest to highest frequency washings per week. I then proceeded to create my needle by created several SVG paths that would draw the needle and that correlate with the washing frequency of a subject. I then created a function that would use a switch statement to select the correct path drawing for the needle depending on the number of washing frequency. 

![guage chart](https://user-images.githubusercontent.com/96400887/177815115-f88b1de7-65f7-4278-b3f6-e7925f345aa5.png)

4. Update all of the plots any time that a new sample is selected: Add an image to the jumbotron,background color , a variety of compatible colors to the webpage
Use a custom font with contrast for the colors.
Add more information about the project as a paragraph on the page.
Create my own layout as shown below:

![full website](https://user-images.githubusercontent.com/96400887/177816342-32d6d1a6-e80e-4f25-89e7-490850964f3f.png)

# Summary

Results, are given by Subject ID and the dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.






