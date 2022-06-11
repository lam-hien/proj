# proj

import pandas as pd

url = "https://github.com/lam-hien/proj/blob/main/2013_plane_flight.csv.gz?raw=tr"

plane_flight = pd.read_csv(url, compression='gzip')
