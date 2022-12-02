# HTTP portfolio

## 1. Write code that executes asynchronously

We used asynchronous JavaScript when fetching data for our project, which displays data relating to countries around the world, including population, currency, land size, capital city, etc. 


## 2. Use callbacks to access values that aren't available synchronously



## 3. Use promises to access values that aren't available synchronously

We carried this out in our fetchData JS file, which contained a function called fetchData that handled promises:

![screenshot(1)](https://user-images.githubusercontent.com/52511353/205361382-43f2dee4-69ff-4bae-8808-0b3a8eb1c83e.png)

## 4. Use the fetch method to make HTTP requests and receive responses

The above-mentioned fetchData JS file used the fetch method to get responses from our two APIs.

![screenshot(1)](https://user-images.githubusercontent.com/52511353/205120422-a4dd07c9-1a5e-4813-8197-a1cb2f6695c0.png)

Our two APIs that we used can be viewed here:

![screenshot(4)](https://user-images.githubusercontent.com/52511353/205127525-a301d416-39a1-4209-8b44-e7694aeff487.png)

## 5. Configure the options argument of the fetch method to make GET and POST requests



## 6. Use the map array method to create a new array containing new values


## 7. Use the filter array method to create a new array with certain values removed


 
## 8. Access DOM nodes using a variety of selectors

The renderReceivedData JS file extensively manipulated DOM nodes using selectors. Each data item for a country (population, currency, capital city etc) had a corresponding class in the HTML. As you can see, these were manipulated, so that the drawn data from the APIs was displayed, within the renderCountry callback function. This was also linked to a separate function, which displayed the weather in the respective country's capital city.   

![screenshot(4)](https://user-images.githubusercontent.com/52511353/205125299-ca3ac2d2-62c2-419b-8922-95cc6debe498.png)

![screenshot(5)](https://user-images.githubusercontent.com/52511353/205125679-9f5945e2-32d1-4b49-86bb-c77210fa9e41.png)


## 9. Add and remove DOM nodes to change the content on the page

Our generateElement JS file not only accessed DOM nodes, but also added and removed them, as you can see in the image below. We created list and paragraph elements, and set attribute and class lists within those elements. In addition, we also appended data in the created list elements.   

![screenshot(2)](https://user-images.githubusercontent.com/52511353/205121567-c727a6f3-ee54-472c-9722-bbc22d64165f.png)

## 10. Toggle the classes applied to DOM nodes to change their CSS properties

As you can see with the screenshot in #9 above, we also created a createLoader function, whose purposes was to gave a visual clue to the user of the website when data was being fetched after the user entered in the name of a country. The function toggled the classes applied to DOM nodes to change their CSS properties. This can be seen in action in the screenshot below, which is what comes up when the user clicks search after entering in a country in the Search bar.

![screenshot(3)](https://user-images.githubusercontent.com/52511353/205122899-ab6879e0-bece-4736-a2ce-7e5a588f293c.png)


## 11. Use consistent layout and spacing



## 12. Follow a spacing guideline to give our app a consistent feel



## 13. Debug client side JS in our web browser



## 14. Use console.log() to help us debug our code

We used console.log regularly to help us debug. It was useful in noting that when there were technical problems, it was often a server side problem at the API's end, rather than issues with our own code. An example can be seen in this screenshot, where the console log reveals that access to fetch from the (frequently erratic) Herokuapp app has been blocked, with the resulting outcome that weather isn't displayed on our page (following screenshot below). Meanwhile, on other occassions, there has been no problems in fetching thi data, and displaying the weather. 

![screenshot(6)](https://user-images.githubusercontent.com/52511353/205364990-00ab849f-2239-4368-94ab-bd7f252384b4.png)
![screenshot(7)](https://user-images.githubusercontent.com/52511353/205365195-3a3241ed-f913-4677-b459-0416e327f20c.png)


