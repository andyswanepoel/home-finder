# Home Finder App

## Problem Statement:

Build an application that will allow a user to search for a home. Users will be able to search based on:
- Number of bedrooms
- Number of bathrooms
- Size
- Location
- Parking

## Components

This is a list of components, in order of importance to the App:

- [x] Search Form (dropdowns)
  - [x] Number of beds
  - [x] Number of baths
  - [x] Size
  - [x] Location
  - [x] Parking
- [X] Table for displaying data
- [ ] Registration
- [ ] Login
- [ ] Routing - could have protected routes to force redirect to login/registration

## Data Storage
In the absence of a database, I'll store the homes in `database.js` file:

```js
    const houses = [
        {
            id: 2,
            location: "tor",
            city: "Toronto",
            province: "Ontario",
            size: "small",
            squarefeet: "485",
            bed: 1,
            bath: 1,
            parking: "true",
            price: 1000000
        },
        ...
    ]
```

## Application Logic

- User enters data on the form
- Frontend validation occurs on inputs, ie:
  - not empty
- Query the "database" to look for any matches
- Display results
- Sort results

## Quick Start

- Clone the repo
- Run `npm install`
- Run `npm start` to start the local server
- Find some homes!