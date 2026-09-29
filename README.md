# Movie Night

A movie discovery website built with HTML, CSS and vanilla JavaScript. Browse a collection of Hollywood thrillers and sci-fi movies, search, filter, sort and save your favourites.

**Live demo:** _add your GitHub Pages / Vercel link here_

## Features

- Movie cards with poster, title, rating, genres and description
- Search by movie title
- Genre filter
- Sort by rating (high to low, low to high)
- Popup with full movie details
- Watchlist (saved in localStorage) with a "My watchlist" filter
- Dark and light mode (remembers your choice)
- Fully responsive layout (CSS Grid)

## Tech Used

- HTML5 (including the `<dialog>` element for the popup)
- CSS3 (Grid, Flexbox, CSS variables for theming)
- JavaScript (DOM manipulation, arrays, event handling, localStorage)

## Project Structure

```
movie-night/
├── index.html      # HTML, CSS and JavaScript in one file
├── posters/        # movie posters (e.g. inception.jpg)
└── README.md
```

## How to Run

1. Download or clone the project.
2. Open `index.html` in any browser.

No installation or build step needed.

## How It Works

- Movies are stored as an array of objects in `index.html`.
- `render()` filters the array (search, genre, watchlist), sorts it, then draws the cards.
- Posters load from `posters/<movie-title-with-dashes>.jpg`. If an image is missing, a gradient card with the title is shown instead.

## Adding a Movie

Add a new object to the `movies` array:

```js
{ id: 9, title: "Movie Name", year: 2020, rating: 8.0, genres: ["Action"], hue: 200, desc: "Short description." }
```

Then add `posters/movie-name.jpg`. The genre button appears automatically.
