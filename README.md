# heros-api
hero test project


## Objective

Create an API that can output some information about heroes using a public superhero api.

## You need:

Create an API that connects to the superhero public API and transforms and extracts the information as specified below.

## Assumptions

- Accept any language or framework that you like or feel more comfortable with.
- Use your creativity to do it the way you think is most efficient.
- The api response should be exactly as we defined it.
- The url must be exactly as we specified.

## Inputs
  - Heroes query api
https://akabab.github.io/superhero-api/

## Necessary methods
When I send a GET request to the */* path, I expect to receive all heroes, but only with id and name in array.

Exemple:

```json
{
  "id": 213,
  "name": "Deadpool"
}
```


When I send a GET request to the path */{powerstat}*, I expect to receive the top 5 superheroes based on the powerstat entered as a parameter.
Example:

GET => /intelligence

```json
[
  {
    "id": 213,
    "name": "Deadpool",
    "intelligence": 80
  },
  {
    "id":333,
    "name" : "Wonder Man",
    "intelligence": 78
  },
  {
    "id":220,
    "name" : "DL Hawkins",
    "intelligence": 69
  },
  ....
  
]
```
