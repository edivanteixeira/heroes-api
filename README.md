# Nstech Jr Backend Challenge

The goal of this test is to assert (to some degree) your coding and architectural skills. You're given a simple problem so you can focus on showcasing development techniques.

You are allowed to use any sort of programming language, framework or library, but be prepared to answer some questions about those libraries, like why you chose them and what other alternatives you're familiar with.

## Objective

Create a REST API that can output data using a public sample api.


## Evaluation Criteria
* The problems are solved efficiently and effectively, the application works as expected
* We expect the api response to be exactly as we defined it
* We expect the provided api url to be exactly as we specified
* The application is well and logically organised
* Following the industry standard style guide
* A git history (even if brief) with clear, concise commit messages
* You demonstrate the knowledge on how to test the critical parts of the application. We do not require 100% coverage.

## Tasks:

* Create an API that connects to the superhero public API
* Extract and transform some information as specified below

### Inputs
  - Heroes query api: https://akabab.github.io/superhero-api/

#### 1- Get All Data
When a GET request is sent to the root path (i.e. http://localhost:8080/), all heroes data should be returned, but only containing id and name.

Example:

```json
[
  {
    "id": 213,
    "name": "Deadpool"
  },
  {
    "id": 123,
    "name": "Batman"
  }
]
```

#### 2- Powerstat Data
When a GET request to the path `/powerstat/{powerstat}`, top 5 data based on the powerstat entered should be returned.

Example:

GET => /powerstat/intelligence

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
