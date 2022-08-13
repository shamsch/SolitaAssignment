# Welcome to my pre-assignment submission for Solita's Dev Academy 2022!

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend

<hr/>

Hi, I am **Shamsur Raza Chowdhury** and this is my pre-assignment submission for Solita's Dev Academy 2022. The code for this assignment is available on two different GitHub repositories:
the Node.js back-end repository is [here](https://github.com/shamsch/city-bike-app-backend) and the React.js front-end repository is [here](https://github.com/shamsch/city-bike-app-frontend). The reason it is split into two repositories is because I initially wanted to create a mobile front-end with React Native, but I later decided to create a web front-end with React.js. You will find the full documentation for the respective repositories in the README.md files located at the root of each repositories. Both, the front and backend, is hosted live on cloud for preview. **Track the progress of the project on the [GitHub project page](https://github.com/users/shamsch/projects/2)** You may also check the issues page of the respective repositories.

<br/>

I hope you enjoy reviewing the code as much as I did planning and developing it. Feel free to reach out to me if you have any questions or if you have any troubles accessing the links to the frontend/backend code bases.

Best regards, <br/>
Shamsur Raza Chowdhury <br/>
August 9th, 2022

**HUOM! Because the app is hosted on free version of Heroku, it goes to sleep after a certain time, so when opening/sending request for the first time, it takes roughly another extra half a minute for it to spin up. Please wait while it does that.**

<hr/>

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend

<hr/>

## Overall Features Implemented:

I tried to implement almost all the features that were mentioned in the [assignment](https://github.com/solita/dev-academy-2022-fall-exercise). Below you can find the complete list of feature that were implemented:

### Data Importing:

- [x] Import data from the CSV files to a database or in-memory storage
  - Imported into a PostgreSQL database hosted on AWS RDS Free tier and in a Docker container if you are using Docker locally to run the backend.
- [x] Validate data before importing
  - Data is validated before importing to the database with a Python script (also a Jupyter Notebook which was initially used) that can be found in the backend repository.
- [x] Don't import journeys that lasted for less than ten seconds
  - Done in `data/validate.ipynb` or `data/script/download_and_validate_data.py` in Docker branch.
- [x] Don't import journeys that covered distances shorter than 10 meters
  - Same as above.

### Journey List View:

- [x] List journeys. If you don't implement pagination, use some hard-coded limit for the list length because showing several million rows would make any browser choke

  - Pagination is implemented in both the frontend and the backend.

- [x] For each journey show departure and return stations, covered distance in kilometers and duration in minutes

  - Implemented in both the frontend and the backend.

  **Extras:**

  - [x] Pagination

    - Backend can be paginated with `?page=<page_number>` parameter on `api/journeys` endpoint. Frontend has a pagination bar that can be used to navigate between pages in the bottom of the page.

  - [x] Ordering per column

    - Backend can be ordered by any column with `?order_by=<column_name>` parameter on `api/journeys` endpoint. Frontend has a dropdown menu that can be used to order the list by any column. You can also set the order direction by adding `?orderDir=<order_direction>` parameter. Read more in the [API Docs.](https://github.com/shamsch/city-bike-app-backend/blob/main/README.md)

  - [x] Searching

    - Backend can be searched by any month, departure station or return station name with `?search=<search_term>` parameter on `api/journeys` endpoint. Frontend has a search bar that can be used to search those said columns.

  - [x] Filtering
    - Backend has multiple filer like maxDistance, maxDuration, minDistance, minDuration. Read more in the [API Docs.](https://github.com/shamsch/city-bike-app-backend/blob/main/README.md). Frontend has those filters implemented visually with a slider.

### Station List View:

- [x] List all the stations

  - Implemented in both the frontend and the backend.

  **Extras:**

  - [x] Pagination
    - Implementation is the same as for the journey list view.
  - [x] Searching
    - Implementation is the same as for the journey list view except for the search is done against the station name.

### Single Station View:

- [x] Station name
  - Station name is shown in the single station request on both the frontend and the backend.
- [x] Station address
  - Same as above.
- [x] Total number of journeys starting from the station
  - Same as above.
- [x] Total number of journeys ending at the station

  - Same as above.

  **Extras:**

  - [x] Station location on the map
    - Backend sends a `static_map_url` property to the frontend with the URL to the static map image. Frontend show the map image and on click redirects to the a map service provider that can show the station location on the map.
  - [x] The average distance of a journey starting from the station
    - Backend sends a `average_departure_distance` property to the frontend with the average distance of a journey starting from the station.
  - [x] The average distance of a journey ending at the station
    - Backend sends a `average_return_distance` property to the frontend with the average distance of a journey ending at the station.
  - [x] Top 5 most popular return stations for journeys starting from the station
    - Backend sends a `top_return_stations` property to the frontend with the top 5 most popular return stations for journeys starting from the station.
  - [x] Top 5 most popular departure stations for journeys ending at the station
    - Backend sends a `top_departure_stations` property to the frontend with the top 5 most popular departure stations for journeys ending at the station.
  - [x] Ability to filter all the calculations per month
    - Backend can be filtered by any month with `?month=<month>` parameter on `api/stations/<station_id>` endpoint. Frontend has a dropdown menu that can be used to filter the calculations per month.

### Additional "Surprise Us With" Features:

- [x] Endpoints to store new journeys data or new bicycle stations
  - Backend has an POST endpoint to store new journeys data with `api/journeys/add` endpoint. Frontend has a form that can be used to store new journeys data.
- [x] Running backend in Docker
  - Backend can be run inside a Docker container. Run `docker-compose up` to start the Docker container. Server will be available on `http://localhost:3001`. Spin up the frontend from `docker-version` branch instead of `main` branch to connect to the backend running in the Docker container. 
- [x] Running backend in Cloud
  - Backend runs on Heroku. Also the database is hosted on AWS RDS. The frontend is hosted with Netlify.
- [ ] Implement E2E tests
- [x] Create UI for adding journeys or bicycle stations
  - Frontend has a form that can be used to add new journeys data or new bicycle stations.

<hr/>

**Links once again for convenience:**

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend
