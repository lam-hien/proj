# proj
Use this [link](https://cran.r-project.org/web/packages/nycflights13/nycflights13.pdf) for feature definition


Data for objective 1:
```
import pandas as pd
url = "https://github.com/lam-hien/proj/blob/main/df.csv.gz?raw=tr"
df = pd.read_csv(url, compression='gzip')
```

Data for objective 2 (this uses the same csv file that Dr. Sadler posted but I've already merged and cleaned it):
```
import pandas as pd
url = "https://github.com/lam-hien/proj/blob/main/2013_plane_flight.csv.gz?raw=tr"
plane_flight = pd.read_csv(url, compression='gzip')
```

Data for objective 3 (2020 & 2021):
```
import pandas as pd

airlines = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/airlines.csv') # same for dallas and atlanta

# flights data
dallas = pd.read_csv('https://github.com/lam-hien/proj/blob/main/dallas_flights.csv.gz?raw=tr', compression='gzip')
atlanta = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atlanta_flights.csv')

# weather data
dallas_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_weather.csv')
atlanta_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atlanta_weather.csv')


# to filter only DAL and DFW destinations from atlanta_flights
atlanta.query("dest == 'DAL' or dest == 'DFW'", inplace=True)

# to filter only IAH destinations from dallas_flights
dallas.query("dest == 'ATL'", inplace=True)
```
