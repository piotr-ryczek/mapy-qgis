# Tworzenie do druku map topograficznych w QGIS w oparciu o OpenStreetMap

## Do poprawy / dopisania

- Siatka NATO (EPSG:326xx) **xx = strefa N**
- Precyzyjny dobór elementów dla mapy topograficznej

## > Program & Podstawowe ustawienia

### Lokalizacja (trzeba otworzyć ręcznie)

`C:\Program Files\QGIS 3.40.7\bin`

`qgis-ltr-bin.exe`

### Ogólne

![Właściwości](./screenshots/wlasciwosci.png)

![Ogólne](./screenshots/ogolne.png)

### Układ Współrzędnych

`EPSG:2180 - ETRF2000-PL / CS92`

![Układ Współrzędnych](./screenshots/uklad_wspolrzednych.png)

### XYZ Tiles

`Dodaj nowe połączenie`

![XYZ Tiles](./screenshots/xyz_tiles.png)

**OpenTopoMap**: `https://tile.opentopomap.org/{z}/{x}/{y}.png`

**OpenStreetMap**: `https://tile.openstreetmap.org/{z}/{x}/{y}.png`

## > Mapa

### Stwórz warstwę

![Nowa warstwa #1](./screenshots/nowa_warstwa.png)

- Plik musi być umieszczony w miejscu dostępnym do zapisu dla QGIS

![Nowa warstwa #2](./screenshots/nowa_warstwa_2.png)

### Rysuj Poligon

![Poligon](./screenshots/poligon.png)

Kliknij **prawym** po zakończeniu rysowania.

### QuickOSM

![QuickOSM #1](./screenshots/quickOSM.png)

![QuickOSM #2](./screenshots/quickOSM_2.png)

**Pobrane warstwy są tymczasowe, po zamknięciu QGIS zostaną utracone.**

## > Siatka

### Tworzenie siatki

![Utwórz siatkę](./screenshots/utworz_siatke.png)

![Ustawienia siatki](./screenshots/ustawienia_siatki.png)

### Odstępy

**A4 = 210mm x 297mm** = 0.21m x 0.297m (**pionowo ułożona kartka** - na wydruku odwrotnie interpretujemy wymiary)

W zalezności od skali. 

> Założmy 1:25 000.

**Poziom**: 0.297m x 25 000 = 7425m

**Pion**: 0.21m x 25 000 = 5250m

> Założmy 1:500

**Poziom**: 0.297m x 500 = 148.5m

**Pion**: 0.21m x 500 = 105m

![Krycie siatki](./screenshots/krycie_siatki.png)

## > Wydruk

### Wydruk

![Nowy wydruk](./screenshots/nowy_wydruk.png)

![Dodaj mapę](./screenshots/wydruk_dodaj_mape.png)

Ewentualnie:

![Atlas widocznosć](./screenshots/widocznosc_atlas.png)

### AtlasGrid

Zaznacz mapę i `Generuj Atlas`. 

![Siatka w wydruku](./screenshots/wydruk_siatka.png)

`Kontrolowane przez Atlas` + `Margines 0%`

![Właściwości elementu](./screenshots/wydruk_wlasciwosci_elementu.png)

Sprawdź poprawność skali:

![Poprawność skali](./screenshots/poprawnosc_skali.png)

### Podziałka

![Podziałka](./screenshots/podzialka.png)

![Ustawienia podziałki](./screenshots/ustawienia_podzialki.png)


### Położenie i rozmiar

`210 - 6 x 2 = 198mm`

`297 - 6 * 2 = 285mm`

![Połóżenie i rozmiar](./screenshots/polozenie_i_rozmiar.png)

**Odstęp siatki dla X i Y**:

`0,016666666667`

![Odstęp i współrzędne](./screenshots/siatka_odstep_i_wspolrzedne.png)

![Czcionka](./screenshots/siatka_czcionka.png)

![Ramka](./screenshots/siatka_ramka.png)

![Oznaczanie współrzędnych](./screenshots/oznaczanie_wspolrzednych.png)


