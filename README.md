# Dni Matematyki 2017
### Warsztaty przygotowane przez KN Gauss

Drodzy studenci!
W tym repozytorium znajdują się dwa pliki:
* *Demo.ipynb* będące notebookiem z przykładami omawianymi na warsztatach 
* *dane_TZ_anon.csv*, gdzie zapisane są rekordy z badania przeprowadzanego przez KN Gauss wśród uczestników Tygodnia Zdrowia na PWr w 2016r.


## Jak pobrać dane
Zasadniczo są dwa sposoby:
* Jeżeli na komputerze masz zainstalowanego gita, możesz w terminalu wpisać:
```
git clone git@github.com:GaussPWr/DniMatematyki2017.git
```
* Jeżeli nie, znajdź przycisk **Clone and Download**, następnie **Download ZIP**

## Jak uruchomić notebook
Aby uruchomić notebook, w folderze **DniMatematyki2017** za pomocą `Shift+PPM` wybierz **Otwórz okno polecenia tutaj** i wpisz komendę `jupyter notebook`

## Jak wczytać dane
Najlepiej będzie, jeżeli w notebooku (Python) skorzystasz z biblioteki *pandas*:
```
import pandas as pd
df = pd.read_csv('dane_TZ_anon.csv', sep=';', encoding='cp1250')
```

## Pomysły?
Zasadniczo zadanie dotyczy pobawienia się z samymi możliwościami biblioteki *bokeh* a nie analizą danych, jednak można poszukiwać zależności między innymi w:
* Zależności między wagą a wzrostem
* Uprawianiem sportu a zdrowiem
* Zdrowiem a godzinami spędzanymi przed komputerem
* Histogram pomiędzy osiaganą średnią a aktywnością studencką

## Zależności
Jeżeli występują u Ciebie problemy z importowaniem bibliotek, musisz z poziomu okna polecenia wywołać:
'''
pip install pandas bokeh==0.12.6
'''
Bądź:
'''
conda install pandas bokeh==0.12.6
'''

Jeżeli nie masz uprawnień administratora, polecenie powinno przyjać formę:
'''
pip install --user pandas bokeh==0.12.6
'''

