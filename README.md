# tooltip-square-js

## Założenia projektowe

* [x] stworzyć dokument html, css oraz js

* [x] stylowanie projektu

* [x] nasłuchiwanie na zdarzenie  `mouseover` i `mouseleave`

* [x] stworzenie funkcji `createTooltip` oraz `removeTooltip` do ww. zdarzeń w `addEventListener`
  
### Tworzenie tooltipa

Stworzenie nasłuchiwania na wszystkie divy po najechaniu. Następnie tworzę funkcje
`createTooltip`, która przyjmuje parametr `e` - parametr `e` jest moim rodzajem
event'u czy to `click`, `mouseover` czy jeszcze inny.
Stworzony  `newTooltip`, który zwraca mi stworzony element `span` i dodaje teraz mój
element `span` do HTML za pomocą `newTooltip.innerHTML`.
Ddodaje za pomocą metody `appendChild` dziecko do mojego rodzica:
- `tooltipParrent.appendChild(newTooltip);`
- rodzic -> `tooltipParrent`
- dziecko -> `newTooltip`
  
### Usuwanie tooltipa

Dodaję nasłuchiwanie za pomocą funkcji `forEach` na każym element, kiedy opuszczę kwadrat - zadziała tutaj zdarzenie `mouseleave` i wykona się funkcja `removeTooltip`;

Funkcja `removeTooltip()` również przyjmuje parametr nasłuchiwania `e`, i usuwa  za pomocą `remove()`
