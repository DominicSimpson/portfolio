# HTTP portfolio

## 1. Write code that executes asynchronously



## 2. Use callbacks to access values that aren't available synchronously


## 3. Use promises to access values that aren't available synchronously


## 4. Use the fetch method to make HTTP requests and receive responses


## 5. Use various tools to check that a website meets accessibility criteria

We ran the HTML through https://validator.w3.org, which is a practice that I used regularly while studying the Advanced Web Authoring module of Birkbeck (indeed, a condition of gaining a high mark there was for the HTML to validate correctly). However, we came up against a number of problems when doing this. The validator flags up trailing slashes on void elements as bad for validation, yet Visual Studio Code (unless I am mistaken) appears to add these trailing slashes automatically. 

![screenshot_accessibility(2)](https://user-images.githubusercontent.com/52511353/203989270-fef2a53c-4985-4db0-93f8-26278b7040d6.png)

In addition, when running the site directly from LiveServer, the Lighthouse function in Chrome confusingly claimed that there were no alt-tags for the images, even though there were, and gave us 91% for Accessibility accordingly.

![screenshot_accessibility(3)](https://user-images.githubusercontent.com/52511353/203996643-bf75a70f-d7be-481e-9a9b-60eeead79e5a.png)

## 6. Ensure a website displays well on screens of different sizes

![screenshot_accessibility(7)](https://user-images.githubusercontent.com/52511353/204137908-110d8d09-db95-4fc0-88e9-8e86f15a72f6.png)

By using HTML elements that naturally adjust to different screen sizes as well as specific styles such as max-width: 100% on images, our page was responsive. We also used flex elements in the CSS.

## 7. Use CSS media queries to ensure content is always presented effectively

We not consider that we needed CSS media queries for this project, as it already scaled well.

## 8. Demonstrate a mobile-first approach to designing a website with a great user experience

Our commits show our mobile-first approach. This is in acknowledgement of the fact that many users increasingly access websites via mobile phone and tablets.

![screenshot_accessibility(6)](https://user-images.githubusercontent.com/52511353/204137741-fabc795d-af8c-4f4b-a2e4-f4d4c79f4a31.png)

## 9. Create an attractive and accessible colour palette for a project

![screenshot_accessibility(8)](https://user-images.githubusercontent.com/52511353/204138184-eec1b4b7-5970-428d-b08c-8197d3431516.png)

We used colour sparingly on the site. There is a black navigation bar, with links in white font colour; then the main section of the site has black font colour against a background of a sombre white/gray ```(#eee8e8)```. Meanwhile, for the biography section, we used a blend of blue, pink, and green to to lift the rider biography cards from the page. 

## 10. Use CSS variables to apply repeated colours to HTML elements

Viewable here, learnt from Founders & Coders' CSS workshop:

![screenshot_accessibility(5)](https://user-images.githubusercontent.com/52511353/204043145-f7215a73-7033-4909-9c63-0f3a4d350d45.png)


