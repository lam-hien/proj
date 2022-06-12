# proj
Use this [link](https://cran.r-project.org/web/packages/nycflights13/nycflights13.pdf) for feature definition


Data for objective 1:
```
import pandas as pd
url = "https://github.com/lam-hien/proj/blob/main/df.csv.gz?raw=tr"
df = pd.read_csv(url, compression='gzip')
```

Data for objective 2:
```
import pandas as pd
url = "https://github.com/lam-hien/proj/blob/main/2013_plane_flight.csv.gz?raw=tr"
plane_flight = pd.read_csv(url, compression='gzip')
```

Data for objective 3:
```
import pandas as pd
dallas_flights = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_flights.csv')
dallas_airlines = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_airlines.csv')
dallas_airports = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_airports.csv')
dallas_planes = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_planes.csv')
dallas_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/dallas_weather.csv')

atl_flights = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_flights.csv')
atl_airlines = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_airlines.csv')
atl_airports = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_airports.csv')
atl_planes = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_planes.csv')
atl_weather = pd.read_csv('https://raw.githubusercontent.com/lam-hien/proj/main/atl_weather.csv')
```
