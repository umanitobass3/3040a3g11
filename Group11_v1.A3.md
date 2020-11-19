# COMP 3040 Assignment 3 - Group 11
  
The API will get the population of a specific city in Manitoba through a single endpoint, with an optional selection of population within a set age range.

## GET /population
### Parameters
- city_name (string)  
  This is the name of the city we want to get the population from.
- min_age (optional) (int)  
  This is the minimum age of a set age range.
- max_age (optional) (int)  
  This is the maximum age of a set age range.

### Resource Descriptions
- population: The total population of the city queried.
- population_within_range: If used, the population within the age range specified.
- status: status indicator

### Example Query
- GET example.com/population?city_name=Winnipeg&max_age=30

### Sample Response
Resource Response:
{
	"results":
	{
    	    "population":"800000",
    	    "population_within_range":"100000",
	},
   	"status":"OK"
}

