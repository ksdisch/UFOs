# UFOs

## Project Overview

### Purpose
The purpose of this project was to create a website wherein users could learn about UFOs. The main feature of this website is a dynamic table presenting the data from data.js, which contains information on many different UFO sightings across the United States. The table contains the date that each sighting occurred, the city, state, and country where it occurred, the shape of the UFO that was sighted, the duration of the sighting, as well as any comments describing the sighting. What makes the table dynamic is that it can filter the occurrences by multiple user inputted criteria. This functionality is demonstrated in the results section below. 

### Resources
- Data Source(s): data.js
- Tools: JavaScript, Bootstrap 3, D3.js library, VSCode

## Results

### Table Filtering Process
The screenshots below demonstrate how the user can filter the table by multiple criteria. There are filters for each column (other than the comments column). If all of the filter fields are blank, the table displays all of the data for each UFO sighting contained within the original dataset in the data.js file as shown in the first screenshot. Once a user inputs a value into one of these filters, the table filters to only show the rows where the value of the filter matches that of the corresponding column as shown in the second screenshot. If another filter value is entered in a different field, the table only shows the rows where both column values match their corresponding filter values, as shown in the third screenshot. This can continue to be done for a third, fourth and fifth filter. 

- #### Unfiltered
Original ![Unfiltered table](/Resources/table-unfiltered.png?raw=true "Title")
- #### One Filter
Original ![One filter table](/Resources/table-one-filter.png?raw=true "Title")
- #### Two Filters
Original ![Two filters table](/Resources/table-two-filters.png?raw=true "Title")

## Summary
Overall, this website is quite functional and informative on UFO sightings. However, there is always room for improvement. Below, I have included one particular drawback I have noticed, as well as two recommendations I have for improving the website.

### Design Drawback
- One drawback I have noticed with the new filters is how sensitive they are, along with not having any guidelines for the user on how to format their filters. For example, "ca" works to filter for sightings that occurred in California, but variations such as "Ca", "CA", or "California " filter out all results and leave the table blank.  

### Recommendations:
- The format of the date column needs to be updated to be more uniform. For example, the dates need to be updated so that all dates are in DD/MM/YYYY format. Right now some are in D/M/YYYY, DD/M/YYYY, or D/MM/YYYY formats. 

 For example, the date filter should instruct the user to input their dates in D/M/YYYY if the day or month 
- The website needs to be updated to set the user up for success when filtering the data. One way of doing this would be to use JavaScript methods to format user inputs to match the data. An example of this would be using the .toLowerCase() method to make any user inputted string all lower case, since that is how the data is formatted. Another way to update the site in this way would be giving the user instructions on how to format their inputs for each filter. A couple ways to do this would be to include tooltips with instructions, and/or including placeholders with correct formatting, such as is included already in the date field.