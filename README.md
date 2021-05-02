# UFOs
#### (Module 11) JavaScript and Dynamic Webpage Development


## OVERVIEW OF PROJECT
### Purpose:  The purpose of the current project was to create a neat, organized, aesthetically-pleasing and, perhaps most importantly, useful presentation of the UFO data collected by Dana to be presented in a simple web-page format with the ability to search through reported UFO sightings using any of 5 descriptor fields (Date, City, State, Country, Shape).

## RESOURCES
  - Data Sources: data.js
  - Software:  JavaScript, D3.js, HTML/CSS/Bootstrap, Chrome DevTools


## RESULTS
#### We have created filters to search by any/each of the 5 UFO-sighting descriptor fields mentioned above (Date, City, State, Country, Shape).  The webpage automatically loads with the full set of sightings data displayed after the introductory article [as shown here](Resources/1_full.png).  

### Searching the sightings data:
#### There are [5 filter boxes](Resources/2_search_boxes.png), each with a phantom entry to show the search format for that field.  To carry out a search, simply enter your search criterion [(e.g., "1/12/2010")](Resources/3_searchbydate.png) into the search box and hit "Enter".  You can refine your search further by entering an additional criterion in another search box [(e.g., "ca" for state)](Resources/4_searchbystate.png), which will then give you results filtered for both criteria.  To revise one of your search criteria, you can simply enter a [new value](Resources/5_revisesearch.png) into the appropriate search box and hit "Enter".

### Clearing a search parameter:
#### To clear one of your UFO-sighting search parameters, click in the appropriate search box, delete it's contents and press "Enter" while the search box is empty (the phantom search example will be visible).  The UFO-sightings data will refresh without that search parameter.

### Resetting the data:
#### To reset the data and clear all search parameters, simply click on ["UFO Sightings"](Resources/6_reset_data.png) in the upper left corner of the webpage, above the "The Truth is Out There" banner.  (Alternatively, you can clear each search parameter one at a time until all search parameters have been reset and only the phantom search examples are shown in the search boxes).


## SUMMARY

### While the webpage is aesthetically pleasing and works well, we do have some drawbacks and suggestions for improvement.

### Drawbacks:
  - Searchers can only search for one date/city/shape/etc at a time.  So, for example, if you want to search for spherically-shaped UFO's, you'd have to do separate searches for ["sphere"](Resources/8_sphere.png), for ["circle"](Resources/7_circle.png) and for ["oval"](Resources/9_oval.png), but you can't currently get them all together. Likewise, you can't specify multiple, cities or states or countries or dates in one search.
  
  - Search boxes need better text contrast (phantom vs search).  While you can see a subtle difference between the phantom search box entries and the actual criteria that have been searched, it's not as clear as it should be.  See [this example](Resources/10_no_contrast.png) of a search for sightings on 1/10/2010 in CA, versus [this example](Resources/10b_no_contrast.png)  which shows the data reset, including phantom search (format) examples of both "1/10/2010" and "ca" in the search boxes.  At a quick glance, you might mistake which search criteria have been executed.
  
  - One final drawback of the current webpage is the limited and static dataset.

### Suggestions for further development:
- Rather than having to enter a blank search, followed by "Enter" in order to clear a search parameter, we'd suggest adding a "clear" button next to each search box.

- We'd also suggest adding a drop-down menu for each search box, populated with the unique choices available for that search criterion in the current data set, so that one doesn't have to keep running searches and getting empty results.

- In addition, we should explore the possibility of including a "keyword" search option for the "Comments" field, because that might help one to find results that are otherwise difficult to isolate.

- And, finally, we'd suggest exploring the possibility of using a dynamic data source in order to have the most current information at hand.  Perhaps linking to an API search would work, if an appropriate source can be found.

