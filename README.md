# UFOs

## Overview of Project
Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, I added table filters for the city, state, country, and shape.

## Resources
- Data Source: data.js
- Software: Python 3.7.6, VS Code

## HTML & app.js Code Updates

**HTML Code Changes**
- I removed the list group that contained the original button
- I added 4 list groups in the container to add the city, state, countyr, and shape filters.
![HTML code](https://user-images.githubusercontent.com/99093289/166167432-263cccab-4916-4dbb-809b-b9f343c9a510.PNG)

**app.js Code Changes**
- I added a filters variable to hold all of the filters as an object
- I created 3 variables for element, value, and filterId 
- I added an if statement to add the filterID and value to the filters list, else clear the filter from the object
- I created a function to filter the table once data is entered (this is where the forEach is used to keep data that matches the filter values)
- Finally, the table is built and an event is added (D3) to listen for the changes to the filtered data.

![app_code](https://user-images.githubusercontent.com/99093289/166167613-477dda52-2059-47fe-abaf-c18b60bca218.PNG)

## Summary
Adding the filters was fairly easy and offers a user friendly interface for whomever will be using this for searching specific UFO sightings. You can enter data you are searching for in one or multiple of the available filters, then press enter for the app to run. The data will populate in the table if the filters match. One drawback of this challenge was by removing the filter button, there is not a clear way to determine how to cleear the filters.

### The Webpage
**Flters**
- These are the filters on the webpage:

![filters](https://user-images.githubusercontent.com/99093289/166167662-3aa79f3b-9f5c-4c66-9bcb-1ad491aaac9e.PNG)

- This is an image of the city, "mason" and state, "oh" being searched:

![multiple_filters](https://user-images.githubusercontent.com/99093289/166167729-72f2f701-efe8-4297-ba66-b129ef72ca75.PNG)

**Recommendations**
- I would recommend adding in a "clear" filter button, as it is slightly confusing on how to clear the filters.
- I would recomend adding in an image under the "UFO Sightings: Fact or Fancy" article heading. There is a large space that looks like the web page is incomplete.


