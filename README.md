# Digi-Biblioteca Project

In the My Digi-Biblioteca project, I create a bookshelf app that allows you to:

* Search for books based on title and author.
* Categorize books you have read, are currently reading, or want to read.

The project emphasizes using React to build the application and provides an API server and client library.

This project [Starter Code](https://github.com/udacity/reactnd-project-myreads-starter) provided from [Udacity](https://www.udacity.com/) as part of [React Nanodegree Program](https://www.udacity.com/course/react-nanodegree--nd019)

## App Install & Usage

To get started using the app:

* Clone the repository `https://github.com/HudaKhalil/Digi-Biblioteca-App.git`
* install all project dependencies with `npm install`
* start the app with `npm start`

## Planning Stage

### UI Mockups Drawings

#### App Main Page

![App Break Each View Into a Hierarchy of Components ](https://github.com/HudaKhalil/Digi-Biblioteca-App/blob/master/src/icons/app_ui_01.JPG)

#### Search Page

![Search Page Break Each View Into a Hierarchy of Components ](https://github.com/HudaKhalil/Digi-Biblioteca-App/blob/master/src/icons/app_ui_02.JPG)

## Backend Server

To simplify your development process, we've provided a backend server for you to develop against. The provided file [`BooksAPI.js`](src/BooksAPI.js) contains the methods you will need to perform necessary operations on the backend:

* [`getAll`](#getall)
* [`update`](#update)
* [`search`](#search)

### `getAll`

Method Signature:

```js
getAll()
```

* Returns a Promise which resolves to a JSON object containing a collection of book objects.
* This collection represents the books currently in the bookshelves in your app.

### `update`

Method Signature:

```js
update(book, shelf)
```

* book: `<Object>` containing at minimum an `id` attribute
* shelf: `<String>` contains one of ["wantToRead", "currentlyReading", "read"]  
* Returns a Promise which resolves to a JSON object containing the response data of the POST request

### `search`

Method Signature:

```js
search(query)
```

* query: `<String>`
* Returns a Promise which resolves to a JSON object containing a collection of a maximum of 20 book objects.
* These books do not know which shelf they are on. They are raw results only. You'll need to make sure that books have the correct state while on the search page.

## Important

The backend API uses a fixed set of cached search results and is limited to a particular set of search terms, which can be found in [SEARCH_TERMS.md](SEARCH_TERMS.md). That list of terms are the _only_ terms that will work with the backend, so don't be surprised if your searches for Basket Weaving or Bubble Wrap don't come back with any results.

## Create React App

This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app). You can find more information on how to perform common tasks [here](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md).

## Contributing

This repository is the starter code for _all_ Udacity students. Therefore, we most likely will not accept pull requests.

For details, check out [CONTRIBUTING.md](CONTRIBUTING.md).
