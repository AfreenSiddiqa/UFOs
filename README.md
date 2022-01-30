# UFOs


##Overview of the project:

  Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria     at the same time. In addition to the date, you’ll add table filters for the city, state, country, and shape.
  
###Deliverable 1:

   Using JavaScript and HTML, I modified the code in my index.html file to create more table filters. In addition to the date filter I created in this module, I added filters for the city, state, country, and shape, as shown in the following image:
   
   ![image](https://user-images.githubusercontent.com/93686963/151681350-8662bccf-2997-45a6-8df4-92cbf3c95e65.png)


I created four more list elements: city, state, country, and shape. These will be similar to the "Enter Date" list element. Each element should have the same "id" as the object properties in the data.js file.
In Step 1 of the app.js file, I created an empty filters variable to keep track of all the elements that change when a search is entered. This variable will be used in Step 5 to store the property “id” and the value that was entered from user input.
Next, I wrote the code for two functions whose names we’ve provided in the starter code, updateFilters() and filterTable().
The updateFilters() function will replace your handleClick() function and update the filters variable you created in Step 1.
The filterTable() function will filter the table data by the value that is entered for the "id" that has changed.
For Step 2, located before the buildTable(tableData) function at the end of the starter code, we will modify the event listener from this module so that it detects a "change" on each input element and calls the updateFilters() function.
In Step 3, I have provided the function, updateFilters(). Inside this function, we will write code in Steps 4-5 to update the filters based on user input.
In Step 4a, I created a variable that saves the element that was changed using d3.select(this).
In Step 4b, I created a variable that saves the value of the changed element’s property.
In Step 4c,I created a variable that saves the attribute of the changed element’s id.
In Step 5, I have written an if-else statement that checks if a value was changed by the user (variable from Step 4b). If a value was changed, add the element’s id (variable from Step 4c) as the property and the value that was changed to the filters variable you created in Step 1. If a value was not entered, then clear the element id from the filters variable.
In Step 6, inside the updateFilters() function, call the filterTable() function that will be used in Step 7.
In the filterTable() function in Step 7, I wrote the  code to filter the table based on the user input that is stored in the filters variable.
In Step 8,I created a variable for the filtered data that is equal to the data that builds the table. This variable will hold the updated table data based on the user input.
In Step 9, I looped through the filters object and store the data that matches the filter values in the variable created in Step 8.
In Step 10, rebuild the table with the filtered data by passing the variable created in Step 8.


###Results:  UFO Sightings!!

![Capture1 - Copy](https://user-images.githubusercontent.com/93686963/151681554-42255929-371b-433c-9162-c9f87b494a95.PNG)

 I added the filters, the page appeared like this when I refreshed it!

![image](https://user-images.githubusercontent.com/93686963/151681350-8662bccf-2997-45a6-8df4-92cbf3c95e65.png)

Finally,when I added or changes the data in the filters, the page appeared like this

![Capture](https://user-images.githubusercontent.com/93686963/151681659-eabbfcec-101a-4e5b-8765-81a2a9835b23.PNG)

![Capture2](https://user-images.githubusercontent.com/93686963/151681664-74249b97-1287-49e9-9c68-fd5c0145bc0d.PNG)


### Drawbacks: 
The user has to know atleast two exact things like (dates or citiy )or (citiy or state) to generate the data in the table and for different countries we has to specify country name beside the city name to generate the data in the table otherwise it will not genetrate the data.

### Recommendations: 
To have more data available like how many people sighted the UFO and the at what time the sighting was visible.
To create additional filter boxes to add the name and contact information of the people who sighted the UFO and their observations which might be helpful in better understanding to the researchers who are studying  and analysing the UFO Sightings.





