# belly-button-challenge

### Why this project?
To build an interactive dashboard to explore the Belly Button Biodiversity dataset, link to an external site that catalogs the microbes that live in human buttons.

### Purpose
To identify the top 10 bacterias present in the average human belly button and compare demographic and location info to determine possible relation.

### Key Aspects of this project
This function creates a bubble and bar chart based on the desired sample. It gets the sample data from the JSON file and extracts the data for the desired ID. It then updates the bubble and bar charts using the out_ids, otu_labels and sample_values data. The otu_id represents the individual on which the test was run to create the data. The otu_labels is the designation that holds the names of the different bacteria. Finally, the the sample_data is the our number value of the bacteria - the ammount observed. The bubble chart is prepared with the otu_ids on the x-axis and sample_values on the y. The hover text is created from otu_labels.<br><br>
The bar chart was created with otu_ids on the y axis labels. The order was reversed to get descending and then sliced the first 10 to get the "Top 10 Bacteria Cultures Found" for our purposes. The sample_values are shown to fill the bars in the chart, also reversed to track with the yticks.
<br><br>
D3 is used to select the dropdown menu with the selDataset ID. It is populated by sample names by appending an option for each sample on the list. buildCharts and buldMetadata functions are called to create the charts. The optionChanged function is created to call up a new sample when it is selected from the dropdown menu. <br><br>

### The instructions for this mini project are divided into the following subsections:
    1 Use the D3 library to read in samples.json from the URL
        https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json
    2 Create a horizontal bar chart with a dropdown menu to display the top 10 OTUs found in that individual.
    3 Create a bubble chart that displays each sample.
    4 Display the sample's metadata, i.e., an individual's demographic information.


### This repo contains the following files:

Root/
 - `samples.json` - Data
 - `README.md` - Provides an overview of the project structure and its contents.
 - `index.html` - html file for exploration and checking progress
    
static/js
 - `app.js` - javascript file where all the work will be completed

### Cited cources, tutorials or helpful readings
following discussions during office hours to get a grasp for starting out<br>
`bar charts -` https://plot.ly/javascript/bar-charts/<br>
`bubble charts` - https://plot.ly/javascript/bubble-charts/<br>
`event listener, changes -` https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events<br>
`dropdown changes for giving option list (need to append my own list through loop) -` https://www.youtube.com/watch?v=_DmdX7e-XRc&ab_channel=CodingShiksha<br>
`js onclick/onchange -` https://www.w3schools.com/js/js_events.asp<br>
`forEach info -` https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
