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

Data for objective 3:
```
import pandas as pd

airlines = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/airlines.csv') # same for dallas and atlanta

dallas_flights = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_flights.csv')
dallas_airports = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_airports.csv')
dallas_planes = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_planes.csv')
dallas_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_weather.csv')

atl_flights = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_flights.csv')
atl_airports = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_airports.csv')
atl_planes = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_planes.csv')
atl_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_weather.csv')

# to filter only DAL and DFW destinations from atlanta_flights
atlanta = atl_flights[(atl_flights['dest'] == 'DAL') | (atl_flights['dest'] == 'DFW')] 

# to filter only IAH destinations from dallas_flights
dallas = dallas_flights[(dallas_flights['dest'] == 'IAH')]
```
