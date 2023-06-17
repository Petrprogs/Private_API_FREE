# 1. Search and get new forecast location id
Base url: https://api.foreca.net/locations/search/searchrequest.json?limit=limit&lang=lang

#### Request params
| URL Parameter       | Description                                               |
| ------------------- | --------------------------------------------------------- |
| searchrequest.json  | Instead of "searchrequest", paste here your search query  |
| limit               | Limit of result items (locations) in response             |
| lang                | Language of response json                                 |

#### Response parsing
| JSON key            | Value description                                          |
| ------------------- | --------------------------------------------------------- |
| query               | Your search query                                         |
| language            | Response language                                         |
| results             | Json array of found locations                             |
| id                  | Id of location for requesting weather forecast            |
| lon                 | Longitude of location                                     |
| lat                 | Latitude of location                                      |
| type                | **?UNKNOWN?**                                             |
| adm1_id-adm3_id     | **?UNKNOWN?**                                             |
| population          | People count of location                                  |
| countryId           | ID of country (short country name)                        |
| timezone            | Time zone of locations                                    |
| preference          | **?UNKNOWN?**                                             |
| warningSources      | Source country of weather warnings??                      |
| name                | Geographical name of location                             |
| countryName         | Short country name                                        |
| countryId           | ID of country (short country name)                        |
| defaultName, defaultCountryName, defaultAdmName | Default names??               |


### Sample request
Request URL: https://api.foreca.net/locations/search/new%20york.json?limit=5&lang=en

Response: 
```
{
  "query": "new york",
  "language": "en",
  "results": [
    {
      "id": "105128581",
      "lon": -74.006,
      "lat": 40.7143,
      "type": "P.PPL",
      "adm1_id": "us.ny",
      "adm2_id": "us.ny.",
      "adm3_id": null,
      "population": 8175133,
      "countryId": "us",
      "timezone": "America/New_York",
      "preference": 237,
      "warningSources": {
        "hurricanes": "us"
      },
      "name": "New York",
      "countryName": "NY",
      "defaultName": "New York",
      "defaultCountryName": "NY",
      "defaultAdmName": "NY",
      "adm1Name": "NY",
      "admName": "NY"
    },
    {
      "id": "102641508",
      "lon": -0.14008,
      "lat": 53.079,
      "type": "P.PPL",
      "adm1_id": "gb.eng",
      "adm2_id": "gb.eng.h7",
      "adm3_id": "gb.eng.h7.32UC",
      "population": 0,
      "countryId": "gb",
      "timezone": "Europe/London",
      "preference": 0,
      "warningSources": {
        "hurricanes": null
      },
      "name": "New York",
      "countryName": "Lincolnshire, United Kingdom",
      "defaultName": "New York",
      "defaultCountryName": "United Kingdom",
      "admName": "Lincolnshire",
      "adm1Name": null
    },
    {
      "id": "104165941",
      "lon": -87.2008,
      "lat": 30.8385,
      "type": "P.PPL",
      "adm1_id": "us.fl",
      "adm2_id": "us.fl.113",
      "adm3_id": null,
      "population": 0,
      "countryId": "us",
      "timezone": "America/Chicago",
      "preference": 0,
      "warningSources": {
        "hurricanes": "us"
      },
      "name": "New York",
      "countryName": "Santa Rosa, FL",
      "defaultName": "New York",
      "defaultCountryName": "Santa Rosa, FL",
      "defaultAdmName": "Santa Rosa, FL",
      "adm1Name": "FL",
      "admName": "Santa Rosa, FL"
    },
    {
      "id": "103489275",
      "lon": -77.1333,
      "lat": 18.1167,
      "type": "P.PPL",
      "adm1_id": "jm.10",
      "adm2_id": "jm.10.1402",
      "adm3_id": null,
      "population": 0,
      "countryId": "jm",
      "timezone": "America/Jamaica",
      "preference": 0,
      "warningSources": {
        "hurricanes": null
      },
      "name": "New York",
      "countryName": "Ewarton, Jamaica",
      "defaultName": "New York",
      "defaultCountryName": "Jamaica",
      "admName": "Ewarton",
      "adm1Name": null
    },
    {
      "id": "104049286",
      "lon": -93.9269,
      "lat": 39.6853,
      "type": "P.PPL",
      "adm1_id": "us.mo",
      "adm2_id": "us.mo.025",
      "adm3_id": "us.mo.025.52400",
      "population": 0,
      "countryId": "us",
      "timezone": "America/Chicago",
      "preference": 0,
      "warningSources": {
        "hurricanes": "us"
      },
      "name": "New York",
      "countryName": "Caldwell, MO",
      "defaultName": "New York",
      "defaultCountryName": "Caldwell, MO",
      "defaultAdmName": "Caldwell, MO",
      "adm1Name": "MO",
      "admName": "Caldwell, MO"
    },
    {
      "id": "103489274",
      "lon": -77.1833,
      "lat": 18.25,
      "type": "P.PPL",
      "adm1_id": "jm.09",
      "adm2_id": "jm.09.635",
      "adm3_id": null,
      "population": 0,
      "countryId": "jm",
      "timezone": "America/Jamaica",
      "preference": 0,
      "warningSources": {
        "hurricanes": null
      },
      "name": "New York",
      "countryName": "Moneague, Jamaica",
      "defaultName": "New York",
      "defaultCountryName": "Jamaica",
      "admName": "Moneague",
      "adm1Name": null
    }
  ]
}
```

# URL for getting all forecast (15mins, hourly, daily, etc.)
https://api.foreca.net/mobile/id_of_location.json

## DOCS WILL BE LITTLE LATER
