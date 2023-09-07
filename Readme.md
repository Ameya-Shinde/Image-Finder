# Image Searcher

## Description

This is a simple Unsplash image searcher application. It allows users to search for images by keyword and view the results.

## To-Do List

- [ ] Add the ability to filter the search results by category.

## How to Use

1. Enter a keyword in the search input field.
2. Click the search button.
3. The results will be displayed in the search results section.
4. Click on an image to view it in full size.
5. Click on Show more button to load more related images.

## JavaScript Functionality

- **accessKey variable:** Stores the Unsplash API key, which is necessary to access the Unsplash API.

- **form element:** Represents the search form. It contains a search-input element and a submit button. The search-input element is where the user enters the keyword to search for. The submit button calls the `searchImages()` function when clicked.

- **searchInput element:** This is the input field where the user enters the keyword to search for.

- **searchResults element:** Serves as the container for the search results. Initially empty, it is populated with images when the `searchImages()` function is called.

- **showMoreBtn element:** Represents the "Show more" button. When clicked, it triggers the `searchImages()` function again to fetch additional search results.

- **searchImages() function:** Responsible for fetching the search results from the Unsplash API. It takes the user-entered keyword as input and returns a list of images.

- **results variable:** Holds a list of objects representing the search results. Each object contains properties like id, urls (for small, medium, and large sizes), and alt_description.

- **map() function:** Iterates over the `results` variable and creates a new `div` element for each image. This `div` element contains an `img` element and an `a` element. The `img` element displays the image, and the `a` element links to the full-size image on the Unsplash website.

- **addEventListener() function:** Attaches an event listener to an element. In this case, the form element's submit event listener is attached to the `searchImages()` function. This means that the `searchImages()` function will be called when the user submits the search form.

- **showMoreBtn element's click event listener:** Also calls the `searchImages()` function. This allows the user to view more search results by clicking the "Show more" button.

## Hosted Link
https://ameya-shinde.github.io/Image-Finder/

