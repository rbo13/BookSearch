# Book Search Demo

**Book List**

![Imgur](http://i.imgur.com/sSINs2zl.png)

**Book Details**

![Imgur](http://i.imgur.com/y9a4AtQl.png)

## Overview

The app does the following:

1. Search a list of books using the [OpenLibrary Search API](https://openlibrary.org/dev/docs/api/search)
2. Display the list of books with their cover images and details
3. Replace ActionBar with Toolbar
4. Use SearchView to search for books with a title
5. Show ProgressBar before each network request
6. Add a detail view to display more information about the selected book from the list
7. Use a share intent to recommend a book to friends

To achieve this, there are five different components in this app:

1. `BookClient` - Responsible for executing the API requests and retrieving the JSON
2. `Book` - Model object responsible for encapsulating the attributes for each individual book
3. `BookAdapter` - Responsible for mapping each `Book` to a particular view layout
4. `BookListActivity` - Responsible for fetching and deserializing the data, configuring the adapter and providing a search interface
5. `BookDetailActivity` - Responsible for providing book detail view and share intent.


## Libraries

This app leverages two third-party libraries:

 * [Android AsyncHTTPClient](http://loopj.com/android-async-http/) - For asynchronous network requests
 * [Picasso](http://square.github.io/picasso/) - For remote image loading

