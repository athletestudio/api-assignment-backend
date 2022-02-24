# Backend Engineering Assignment
### Overview
The goal of this assignment is to aggregate data from multiple API endpoints to create a revised `athlete` object which we will store in a NoSQL database.

Create a new project locally and write a JavaScript or Python function to extract data from each athlete's individual API endpoint listed here:

`https://sports.core.api.espn.com/v2/sports/football/leagues/nfl/athletes`

The new object should contain the following data:

```
{
  "id": "",
  "firstName": "",
  "lastName": "",
  "fullName": "",
  "age":"",
  "age_label": "",
  "team": {
    "name": "",
    "location": "",
    "displayName: "",
    "color": "",
    "alternateColor": ""
  }
}
```

Setup MongoDB (or another NoSQL database) to store each newly formatted object.

`age_label` is a new data field which should be dynamically set as `Senior` or `Junior` for each athlete. Set the value to `Senior` if the athlete's age is equal to or greater than the average athlete age across the entire league. Set the value to `Junior` if the athlete's age is below the average athlete age across the entire league.

Deliver the project files via Github with instructions to run the application locally.
