# html

Język HTML to język, który za pomocą **znaczników**, inaczej zwanych **tagami**, opisuje strukturę strony i jej zawartość.
Poniżej mamy przykład startowej struktury pliku html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
> [!TIP]
> W edytorze Visual Studio Code w pustym pliku html strukturę startową można w szybki sposób wygenerować wpisując **!** i klawisz Tab

Dokument składa się z dwóch podstawowych części:
- Head pomiędzy znacznikami ```<head> </head>``` gdzie wpisujemy informacje dla przeglądarki. Występują tam znaczniki ```<meta>```oznaczające metadane wpisywane w atrybutach tych znaczników np. ```charset="UTF-8"``` oznaczający rodzaj stosowanej tablicy znaków.
- Body pomiędzy znacznikami ```<body> </body>``` gdzie wpisujemy zawartość strony. Tam będą znaczniki wraz z zawartością.

## Podstawowe znaczniki html
### Nagłówki od h1 do h6
```html
<h1>Zwiedzamy świat</h1>
<h2>Piramidy w Gizie</h2>
```
### Akapit
```html
<p>Przykład akapitu</p>
<p>Tu kolejny akapit</p>
```
### Grafika
```html
<img src="obraz.jpg">
```
### Hiperłącze (link)
Poniżej przykład linku do strony z atrybutem **target**.
```html
<a href="https://oi.edu.pl" target="_blank">Olimpiada Informatyczna</a>
```
### Tabele
Tabela zawiera się pomiędzy znacznikami ```<table> </table>```, w obrębie tabeli mamy wiersze ```<tr> </tr>``` a w wierszach komórki ```<th> </th>``` dla nagłówków i ```<td> </td>``` dla danych.
```html
<table border="1">
        <tr>
            <th colspan="2">Piramidy w Gizie</th>
        </tr>
        <tr>
            <th>Nazwa Piramidy</th>
            <th>Wysokość</th>
        </tr>
        <tr>
            <td>Cheopsa</td>
            <td>147 metrów</td>
        </tr>
        <tr>
            <td>Chefrena</td>
            <td>137 metrów</td>
        </tr>
        <tr>
            <td>Mykerinosa</td>
            <td>65 metrów</td>
        </tr>
    </table>
```
### Listy
W języku html możemy utworzyć listy numerowane ```<ol> </ol>``` lub wypunktowane ```<ul> </ul>```. Elementy listy dla obu rodzajów są pomiędzy znacznikami ```<li> </li>```.
```html
<h2>Ciekawe miejsca do odwiedzenia</h2>
    <ol>
        <li>Wieża Eiffla w Paryżu</li>
        <li>Krzywa Wieża w Pizie</li>
        <li>Koloseum w Rzymie</li>
    </ol>
    <ul>
        <li>Łazienki Królewskie w Warszawie</li>
        <li>Machu Picchu w Peru</li>
        <li>Wielki Kanion w USA</li>
    </ul>
```

## CSS Kaskadowe arkusze stylów
Dzieki stylom możemy opisać wygląd strony. Sytle zapiszemy w osobntm pliku np. **style.css**. Budowa pliku css polega na odwoływaniu się do znaczników, klas lub indeksów i wpisywaniu dla nich parametrów.

Przykład dla znacznika ```<p>```:
```css
p {
  text-align: center;
  color: red;
}
```
Znaczniki html mogą posiadać klasy np. ```<h1 class="title">Tytuł</h1>``` wówczas w css odwołujemy się do tej kasy pisząc kropkę i nazwa klasy.
```css
.title {
  text-align: center;
  color: green;
}
```
Dla indeksu piszemy # i nazwa indeksu. Przykład dla ```<h1 id="start">Tytuł</h1>```
```css
#start {
  text-align: center;
  color: blue;
}
```

