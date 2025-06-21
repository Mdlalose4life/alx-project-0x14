# alx-project-0x14

## API Overview

The **MoviesDatabase API** is a robust and comprehensive interface that provides access to information on over 9 million titles—including movies, TV shows, and episodes—and more than 11 million actors, crew, and cast members. It includes detailed metadata such as biographies, ratings, trailers (via YouTube), awards, and more. This API is ideal for developers building movie-related apps, platforms, or tools that require accurate, up-to-date data.

## Version

**v1** – The current version as per the API documentation.

## Available Endpoints

### Titles
- **GET /titles**: Returns a list of titles based on filters and sorting options.
- **GET /x/titles-by-ids**: Returns a list of titles by an array of IMDb IDs.
- **GET /titles/{id}**: Fetches detailed information about a single title using its IMDb ID.
- **GET /titles/{id}/ratings**: Retrieves rating and vote count for a specific title.

### Episodes and Seasons
- **GET /titles/series/{id}**: Returns episodes of a series with ID and episode details.
- **GET /titles/seasons/{id}**: Returns the number of seasons for a given series.
- **GET /titles/series/{id}/{season}**: Returns all episodes of a specific season.
- **GET /titles/episode/{id}**: Returns detailed info about a specific episode.

### Search
- **GET /titles/search/keyword/{keyword}**: Search titles by keyword.
- **GET /titles/search/title/{title}**: Search titles by full or partial name.
- **GET /titles/search/akas/{aka}**: Search titles by alternate names (AKAs).

### Upcoming
- **GET /titles/x/upcoming**: Fetches a list of upcoming titles based on filters.

### Actors
- **GET /actors**: Returns a paginated list of actors.
- **GET /actors/{id}**: Fetches detailed info about an actor by IMDb ID.

### Utils
- **GET /title/utils/titleType**: Lists available title types.
- **GET /title/utils/lists**: Lists available collections like top-rated or popular titles.
- **GET /title/utils/genres**: Lists genres available in the database.

## Request and Response Format

All requests are made via HTTPS using `GET` requests. Query parameters are optional for most endpoints.
