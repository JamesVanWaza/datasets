# Devcon 2020 Developer Workshop dataset

Welcome to the Algolia Devcon 2023 repository for the "Algolia 101: A comprehensive and hands-on developer training from Data Ingestion to Front-End" Workshop.

## What is this repository?

This repository contains the dataset that will be used during the workshop. It is a subset of the [IMDB](https://www.imdb.com/) dataset, containing about 10K movies.

## How to use it?

The dataset is available in the `data` folder. It is a JSON file containing an array of objects, each object representing a movie.
You can import it directly using Algolia's Dashboard or API.

## Shared Application ID and API Keys

For the purpose of this workshop, we have created two Algolia applications that you can use to import the dataset and follow along the workshop. Those Applications will be deleted 1 week after the workshop.

### US located cluster

APP ID: YS0MNKGIQM
Admin API Key: dc900991cad38d36dbbfb682f7bf3aa8
Read API Key: 544c9265d256129a6397d541860df1ae


### EU located cluster

APP ID: QDDE6ECCK1
Admin API Key: 5a57f4724517e284a2bc3a588a1ef71d
Read API Key: 7a291ee30130c6b303b301d04d270a2c

## CSS File

You will see a css file named App.css. You will be asked to download the file and place it in the appropriate location for the front-end workshop. React Applications will keep the name App.css and Vanilla JS applications will rename it to styles.css. 

## Snippets

During the UI live coding sessions, your presenter may suggest you copy paste the following bits of boilerplate to avoid having to manually type them:

Basic HTML page boilerplate
```HTML
<!DOCTYPE html>
<html>
  <head>
    <title>InstantSearch Demo</title>
    <meta charset="UTF-8" />
  </head>

  <body>
    <script src="src/index.js"></script>
  </body>
</html>
```

Markup template to work with the provided CSS:
```HTML
<div class="header">
  <div class="header-wrapper">
    <div class="header-nav">
      <h3>Home</h3>
    </div>
    <!-- Searchbox goes here -->
  </div>
</div>
<div class="container">
  <div>
    <!-- Refinementlist goes here -->
  </div>
  <div>
    <!-- Hits go here -->
    <!-- Pagination goes here -->
  </div>
</div>
```

Basic (Vanilla JS) hit template:
```JS
<div class="items">
  <img src="https://image.tmdb.org/t/p/w185${hit.poster}" alt=${hit.title} />

  <div class="items-info">
    <div class="items-info--title">
      <h3>
        ${hit.title}
      </h3>
    </div>
    <div className="items-info--genres">
      <span className="genre-title">${hit.genres[0]} - ${hit.vote_average}</span>
    </div>
  </div>
</div>
```
