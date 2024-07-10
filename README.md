# belly-button-challenge

3rd party code sources:
  Chat gpt
  EdX tutor

  index.html:
    imports dependencies: d3, plotly, etc
    create site layout and elements

  apps.js:
    -function buildMetadata(sample)
      performs d3 api request for json sample data, links to html file and updates site table with data matching the id selected from the dropdown
    -function buildCharts(sample)
      performs api request for data based on selection from dropdown tab, data is then used to build and render a bar and bubble chart
    -function init():
      performs api request, selecting the 'name' field from the json data and then appending the dropdown element in the html file with each 'name' extract along with a new 'option' element and 'value' tag. initializes the site with the first sample extracted to generate a populated data table and graphs
    -function optionChanged(newSample):
      initializes the buildsCharts function based on events triggered by user activity, takes the user selection from the dropdown menu specified in the html file and triggers the graphing functions to process a new set of data
      
      
    
