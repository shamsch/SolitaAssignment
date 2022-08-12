# Welcome to my pre-assignment submission for Solita's Dev Academy 2022!

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend

<hr/>

**HUOM! Still a work in progress, check after 14th August for final version :)**

<br/>

Hi, I am **Shamsur Raza Chowdhury** and this is my pre-assignment submission for Solita's Dev Academy 2022. The code for this assignment is available on two different GitHub repositories:
the Node.js back-end repository is [here](https://github.com/shamsch/city-bike-app-backend) and the React.js front-end repository is [here](https://github.com/shamsch/city-bike-app-frontend). The reason it is split into two repositories is because I initially wanted to create a mobile front-end with React Native, but I later decided to create a web front-end with React.js. You will find the full documentation for the respective repositories in the README.md files located at the root of each repositories. Both, the front and backend, is hosted live on cloud for preview. **Track the progress of the project on the [GitHub project page](https://github.com/users/shamsch/projects/2)** You may also check the issues page of the respective repositories.

<br/>

I hope you enjoy reviewing the code as much as I did planning and developing it. Feel free to reach out to me if you have any questions or if you have any troubles accessing the links to the frontend/backend code bases.

Best regards, <br/>
Shamsur Raza Chowdhury <br/>
August 9th, 2022

<hr/>

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend

<hr/>

## Overall Features Implemented:

I tried to implement almost all the features that were mentioned in the [assignment](https://github.com/solita/dev-academy-2022-fall-exercise). Below you can find the complete list of feature that were implemented:

### Data Importing:

- [x] Import data from the CSV files to a database or in-memory storage
- [x] Validate data before importing
- [x] Don't import journeys that lasted for less than ten seconds
- [x] Don't import journeys that covered distances shorter than 10 meters

### Journey List View:

- [x] List journeys. If you don't implement pagination, use some hard-coded limit for the list length because showing several million rows would make any browser choke

- [x] For each journey show departure and return stations, covered distance in kilometers and duration in minutes

  **Extras:**

  - [x] Pagination

  - [x] Ordering per column

  - [x] Searching

  - [x] Filtering

### Station List View:

- [x] List all the stations

  **Extras:**

  - [x] Pagination
  - [x] Searching

### Single Station View:

- [x] Station name
- [x] Station address
- [x] Total number of journeys starting from the station
- [x] Total number of journeys ending at the station

  **Extras:**

  - [x] Station location on the map
  - [x] The average distance of a journey starting from the station
  - [x] The average distance of a journey ending at the station
  - [x] Top 5 most popular return stations for journeys starting from the station
  - [x] Top 5 most popular departure stations for journeys ending at the station
  - [x] Ability to filter all the calculations per month

### Additional "Surprise Us With" Features:

- [x] Endpoints to store new journeys data or new bicycle stations
- [x] Running backend in Docker
- [x] Running backend in Cloud
- [ ] Implement E2E tests
- [x] Create UI for adding journeys or bicycle stations

<hr/>

**Links once again for convenience:**

### Front-end codebase: https://github.com/shamsch/city-bike-app-frontend

### Back-end codebase: https://github.com/shamsch/city-bike-app-backend
