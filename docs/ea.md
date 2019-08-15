# External Adapters

In order to help the development of the Chainlink ecosystem, we are continually developing external adapters to help connect users and data. Below you will find our current publicly available adapters.

## Open Weather External Adapter
This adaptor allows nodes to support the Open Weather API (https://openweathermap.org/api). It was built using the Chainlink NodeJS Template available at https://github.com/thodges-gh/CL-EA-NodeJS-Template.

A full setup and install guide, as well as source code, is available at: https://github.com/securedatalinks/CLAdaptor-OpenWeather


### Supported Parameters / Endpoint
The following API endpoints are supported with the related parameters. Note CityId is a ID specific to the Open Weather API. To Find the CityID for any city, visit http://bulk.openweathermap.org/sample/city.list.json.gz

- Current Weather Data
    - Endpoint: weather
    - Params
        - CityId: The City ID to get data for

- Forcasted Weather Data
    - Endpoint: forecast
    - Params
        - CityId: The City ID to get data for
        - Days: The number of days to get data for (up to 5 days)

The following premium API endpoints are also supported

- Forcasted Weather Data (Hourly)
    - Endpoint: forecast/hourly
    - Params
        - CityId: The City ID to get data for
        - Days: The number of days to get data for (up to 4 days)

- Forcasted Weather Data (16 Days)
    - Endpoint: forecast/daily
    - Params
        - CityId: The City ID to get data for
        - Days: The number of days to get data for (up to 16 days)

- Climate Forecast Weather Data (Month)
    - Endpoint: climate/monthly
    - Params
        - CityId: The City ID to get data for