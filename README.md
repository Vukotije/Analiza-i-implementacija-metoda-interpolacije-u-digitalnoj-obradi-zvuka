# Analiza-i-implementacija-metoda-interpolacije-u-digitalnoj-obradi-zvuka
Project for extra credit in course of "Numerical algorithms and numerical software"

## Kratak opis problema

Zvuk je jedan od najčešće konzumiranih vidova sadržaja koje čovek susreće u svojoj svakodnevnici, bila to muzika, govor ili bilo koji drugi propratni sadržaj drugih medija. Zbog toliko velike i široke interakcije sa zvukom veoma nam je bitno da njegov kvalitet bude na što većem nivou uz to da njegovo zauzeće memorijskog prostora ne bude previše bahato. Kako je zvuk u svom fizičkom stanju analogni talas, a njegova reprezentacija u kompjuteru je digitalna, moramo izgubiti određenu količinu podataka. U tom transferu u digitalni zapis analognog zvuka mogu nastati problemi, poput gubitka kvaliteta i potrebe za rekonstrukcijom oštećenih delova. Interpolacija, kao ključna tehnika u ovakvim situacijama, omogućava da se popune nedostajući podaci i unapredi kvalitet zvučnog signala. Istraživanje različitih metoda interpolacije može pomoći u boljem razumevanju njihovih prednosti i ograničenja u specifičnim primenama. Cilj ovog projekta je istražiti i implementirati metode interpolacije, analizirati i predstaviti njihov uticaj na kvalitet digitalnog zvuka u različitim scenarijima.

## Metodologija

Projekat će se fokusirati na implementaciju i poređenje metoda interpolacije u kontekstu rekonstrukcije i skaliranja frekvencije. Osnovne faze projekta:

### Priprema audio podataka za interpolaciju
- Priprema audio snimaka sa oštećenim segmentima koji zahtevaju rekonstrukciju.
- Priprema audio snimaka sa niskom frekvencijom na kojima će se primeniti skaliranje na više frekvencije.

### Implementacija metoda interpolacije
- **Linearna interpolacija**: Osnovna metoda koja povezuje podatke pravolinijski.
- **Kubna i splajn interpolacija**: Glatkije metode koje koriste krive za preciznije prilagođavanje signalu.
- **Lanczos metoda**: Pogodna za skaliranje signala.
- **Polinomska interpolacija**: Pogodna za kompleksnije oblike signala.

### Kreiranje modela za poređenje
- Svaka metoda će biti implementirana i testirana na istim podacima kako bi se omogućila objektivna procena rezultata.
- Rezultati će biti analizirani i evaluirani na više različitih načina uzimajući u obzir različite primene interpolacije.

### Evaluacija i prezentovanje rezultata

## Skup podataka

Za istraživanje i evaluaciju koristiće se sledeći skupovi podataka:
- Audio snimci različitih žanrova i frekvencija uzorkovanja (8 kHz, 16 kHz, 44.1 kHz)

Svi podaci će biti pažljivo izabrani kako bi uključivali različite izazove, poput oštećenja, nedostajućih uzoraka i šumova. 

**Mogući izvori podataka su:**
- [https://archive.org/search?query=mediatype%3A%28audio%29](https://archive.org/search?query=mediatype%3A%28audio%29)
- [https://www.openslr.org/index.html](https://www.openslr.org/index.html)
- [https://archive.org/details/Greatest_Speeches_of_the_20th_Century](https://archive.org/details/Greatest_Speeches_of_the_20th_Century)
- [https://research.google.com/audioset/](https://research.google.com/audioset/)

## Način evaluacije

Evaluacija implementiranih metoda interpolacije vršiće se kroz sledeće pristupe:

### Objektivne metrike
- **Signal-to-Noise Ratio (SNR)**: Ocenjuje koliko je interpolirani signal približan originalnom.
- **Mean Squared Error (MSE)**: Kvantifikuje grešku između interpoliranog i originalnog signala.

### Subjektivne procene
- **ABX testovi**: Korisnici će slušati izlazne audio fajlove i uveriti se u razlike i zaključke analize.

### Poređenje metoda
- Rezultati različitih metoda će biti međusobno upoređeni kako bi se utvrdile prednosti i nedostaci svake metode u određenim scenarijima.

## Tehnologije

Za realizaciju projekta koristiće se:
- **Programski jezik**: Python 3.12.

### Biblioteke
- **NumPy** za numeričke proračune.
- **SciPy** za implementaciju interpolacionih metoda.
- **LibROSA** za procesiranje audio signala.
- **Matplotlib** za vizualizaciju rezultata.

## Navođenje materijala/literature

- Lynn Blair, "Data interpolation and its effects on Digital Sound Quality": [https://www.yumpu.com/en/document/read/50679011/data-interpolation-and-its-effects-on-digital-sound-quality-mcmurry-](https://www.yumpu.com/en/document/read/50679011/data-interpolation-and-its-effects-on-digital-sound-quality-mcmurry-)
- Python biblioteke za procesiranje audio signala: [http://eprints.maynoothuniversity.ie/4115/1/40.pdf](http://eprints.maynoothuniversity.ie/4115/1/40.pdf)
- SciPy dokumentacija za interpolaciju: [https://docs.scipy.org/doc/scipy/reference/interpolate.html](https://docs.scipy.org/doc/scipy/reference/interpolate.html)
- NumPy dokumentacija: [https://numpy.org/doc/stable/user/index.html](https://numpy.org/doc/stable/user/index.html)
- Sound on Sound. (April 2012). "What data compression does your music": [https://www.soundonsound.com/techniques/what-data-compression-does-your-music](https://www.soundonsound.com/techniques/what-data-compression-does-your-music)
- Claude, Duchon (1979-08-01). "Lanczos Filtering in One and Two Dimensions": [https://doi.org/10.1175/1520-0450(1979)018<1016:LFIOAT>2.0.CO;2](https://doi.org/10.1175/1520-0450(1979)018%3C1016:LFIOAT%3E2.0.CO;2)

---

**NANS, SV-2023, Vukan Radojević**
