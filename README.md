# Scraping-with-Python-and-BS-1
We will do scraping from multiples webpages using Python and Beautifulsoup
# Importing the libraries
import pandas as pd
import numpy as np
import requests
from bs4 import BeautifulSoup
from time import sleep
from random import randint

# declaring the headers
headers = {"Accept language":"en-US, en; q=0.5}

# declaring the list of empty variables
WebPage = []
Brand = []
Model = []
Price = []
Price_pix = []
Caliber = []
Disponivel = []
Esgotado = []
Pistola = []
Revolver = []
Carabina = []

# creating an array of values and passit it in the url for dynamic webpages
pages = np.arange(1, 1000, 100)

# list of webpages
# https://gatilhoarmas.com.br
# https://beartac.com.br
# https://guntrade.com.br
# https://www.armasriopreto.com.br/
# https://www.falconarmasdefogo.com.br/
# https://www.casadotiro.com.br/
# https://www.azdeespadas.com.br/
# https://gatilhoarmas.com.br/
# https://www.pescaeciaarmas.com.br/
# https://artgun.com.br/
# https://www.lojanorisk.com/
# https://lorguns.com.br/
# https://www.tactical.com.br/

# the core of the script
