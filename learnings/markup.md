# Markup portfolio

## 1. Structure a site using semantic HTML to aid accessibility

![screenshot_accessibility](https://user-images.githubusercontent.com/52511353/203984380-4f7c734a-79ee-4f48-9c70-fdfe18bffbaa.png)

This screenshot shows that we incorporated semantic elements in our HTML, including demarcating each section so that it can be tabbed through by the user, as well as H1 and H2 headings in correct order, which ensured that they would be read out by a screen reader (see below). In addition, we used alt-tags on each image.
Being able to tab through the site is especially important for those with sight access requirements, and relates to the below.
Unfortunately, we missed using ARIA-labels, which was a glaring omission. 

## 2. Make a web page more readable for screen readers

After incorporating the semantic elements in point 1, I then tested the site via screen readers such as Windows Narrator, Speechify, and NVDA. The site worked well with the first two, but came up against issues with NVDA, which appeared to not be able to read the semantic HTML well. 

## 3. Design a UI without relying solely on colour, so that we don’t exclude colour-blind users

![screenshot_accessibility(4)](https://user-images.githubusercontent.com/52511353/204042160-5571f419-7259-46ea-8a39-ce097b0c4b5c.png)

## 4. Ensure our UI has sufficient colour contrast so that everyone can perceive it comfortably

## 5. Use various tools to check that a website meets accessibility criteria

We ran the HTML through https://validator.w3.org, which is a practice that I used regularly while studying the Advanced Web Authoring module of Birkbeck (indeed, a condition of gaining a high mark there was for the HTML to validate correctly). However, we came up against a number of problems when doing this. The validator flags up trailing slashes on void elements as bad for validation, yet Visual Studio Code (unless I am mistaken) appears to add these trailing slashes automatically. 

![screenshot_accessibility(2)](https://user-images.githubusercontent.com/52511353/203989270-fef2a53c-4985-4db0-93f8-26278b7040d6.png)

In addition, when running the site directly from LiveServer, the Lighthouse function in Chrome confusingly claimed that there were no alt-tags for the images, even though there were, and gave us 91% for Accessibility accordingly.

![screenshot_accessibility(3)](https://user-images.githubusercontent.com/52511353/203996643-bf75a70f-d7be-481e-9a9b-60eeead79e5a.png)

## 6. Ensure a website displays well on screens of different sizes

## 7. Use CSS media queries to ensure content is always presented effectively

## 8. Demonstrate a mobile-first approach to designing a website with a great user experience

## 9. Create an attractive and accessible colour palette for a project

## 10. Use CSS variables to apply repeated colours to HTML elements




