# WTF!? Kurse / Web

## Willkommen im **(Exzellenz)kurs**

Ay, Ay! :v: Willkommen in unserem Python Kurs im Sommersemester 2018/19. Bevor es losgeht, ein paar Details zu unserem Kurs

* Donnerstags, 3. DS
* Ort: APB/E046
* Kursseite: www.html5.wtf

Unser Kurs besteht aus drei Komponenten

<div class="panel color-1">
Präsentation
</div>

<div class="panel color-2">
Skript
</div>

<div class="panel color-3">
Praxisaufgabe
</div>

Sämtliche Slides sowie Praxisaufgaben findest du auf der Kursinternetseite der jeweiligen Kurseinheit zum Download bereit. Das Skript ist separat auf der Webseite erreichbar.

!> Für das Sammeln von Credits ist ein Nutzerkonto auf unserer Kursseite erforderlich. Eine Freischaltung erfolgt über https://wtfkurse.de/web/enroll.

### Kurstutoren

<div class="teacher-list">
	<div class="teacher">
		<div class="avatar">
      <img src="https://wtfkurse.de/wp-content/themes/wtfkurse/img/teacher/tutor_patrik.png">
		</div>
		<div class="contact">
			<h4>Patrik Phan</h4>
			patrik@wtfkurse.de
		</div>
	</div>
	<div class="teacher">
		<div class="avatar">
      <img src="https://wtfkurse.de/wp-content/themes/wtfkurse/img/teacher/tutor_kevin.png">
		</div>
		<div class="contact">
			<h4>Kevin Schmid</h4>
			kevin@wtfkurse.de
		</div>
	</div>
</div>

## Grundlagen **Entwicklung**

### Grundbegriffe

<div class="column-2">
	<div>
	<strong>Tags</strong><br>engl. für Etiketten und stehen im HTML-Quelltext für einzelne Elemente/Befehle.
	</div>
  <div>
	<strong>Attribute</strong><br>Attribute sind zusätzliche Eigenschaften.
	</div>
	<div>
	<strong>Editor</strong><br>Ein Editor ist eine Software zur Bearbeitung und Eingabe von Programmcode (Quelltext). Er unterscheidet sich von einer komfortablen Textverarbeitung dadurch, dass er keine unsichtbaren Formatierungsanweisungen in den Text einfügt, um ihn Absätze, Listen und Tabellen zu gliedern.
	</div>
	<div>
	<strong>IDE</strong><br>Eine IDE ist eine Integrierte Entwicklungsumgebung (Abk. für Integrated Development Environment) und vereint Editor, Compiler und Debugger unter einer einheitlichen Oberfläche.
	</div>
  <div>
	<strong>Webserver</strong><br>Ein Webserver ist ein Dienst, der zur Auslieferung von (Web-)Dokumenten auf einem Server dient.
	</div>
  <div>
	<strong>FTP</strong><br>FTP (Abk. für File Transfer Protocol) dient zur Dateiübertragung zwischen einem Client und einem Server.
	</div>
</div>


### HTML im Kurzportrait

Die Websprache HTML (Abk. für Hypertext Markup Language) liegt mittlerweile in der fünften Verfassung vor. Zuvor sollte das parallel entwickelte XHTML2-Standart erscheinen. Das Standardisierungskonsortium W3C verkündete allerdings im Juli 2009, dass die Arbeiten dafür eingestellt werden, damit alle freien Ressourcen bei HTML5 liegen.

?> Das Konsortium „W3C“ ist das Gremium zur Standardisierung der Webtechnologien. Es legt die allgemeinen Richtlinien und Spezifikationen für HTML, XHTML, XML, RDF, OWL, CSS, SVG und WCAG fest.

Am 28. Oktober 2014 legte W3C die fertigen HTML5-Spezifikationen vor. HTML5 ist damit der offizielle Nachfolger von HTML4. Folglich endete mit der Einführung die Ära von HTML 4.01, XHTML 1.0 und DOM HTML.

Der neue Webstandard unterstützt Multimediainhalte wie Video und Audio oder die Möglichkeit eines lokalen Speichers. Hierfür benötigte man zuvor oft zusätzliche Anwendungen wie Adobe Flash. Im Zuge der Aktualisierung wurden auch weitere HTML-Elemente für ein Layout technisches Gestalten eingeführt. Dazu zählen `section`, `nav`, `article`, `aside`, `header` sowie `footer`.

HTML5 wird heute oft in Kombination mit CSS3, der dritten Generation von CSS, verwendet. „CSS Level 3“ ist seit dem Jahr 2000 in Entwicklung. 

## Einführung in **HTML5/CSS**

### HTML5 Boilerplate

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="utf-8">
    <title>Seitentitel</title>
</head>
<body>

</body>
</html>
```

#### Aufbau
Der Aufbau von HTML lässt sich einfach mit dem Aufbau eines Menschen vergleichen. Es gibt innerhalb vom HTML-Tag einen Kopf- und einen Körperbereich.

Im _Kopfbereich_ (`<head>`) befindet sich die Identität der Webseite: Titel, Zeichenkodierung, Beschreibung. Diese werden durch sogenannte „Metatags“ definiert. 

Im _Körperbereich_ (`<body>`) werden sämtliche Inhalte definiert. Hier werden sämtliche HTML-Elemente (Tags) implementiert.

Grundsätzlich bestehen HTML-Quelltexte aus Tags. Tags sind HTML Befehle, die in spitzen Klammen stehen und grundsätzlich kleingeschrieben werden.

Jeder HTML-Befehl hat die Form `<tag>`, der schließende Tag am Ende `</tag>`

#### Schachteln von HTML-Befehle

Bei der Reihenfolge der HTML-Befehle muss darauf geachtet werden, dass diese in umgekehrter Reihenfolge wieder geschlossen werden.

```html
<tag1> <tag2> Inhalt </tag2> </tag1> 
```

Für die verschiedenen Tags empfiehlt sich ein „Cheatsheet“ als Überblick.

#### Attribute in HTML-Tags

Mittels Attribute lassen sich HTML-Befehle näher spezifizieren. 

```html
<tag attribut="wert">
```

### Cascading Style Sheets (CSS)

Die Webtechnologie CSS ist die professionelle Art der Gestaltung und Formatierung von HTML-Elementen. Damit lässt sich Layout vom Inhalt trennen und deutlich effizienter verwalten. Sie lässt sich nur in Kombination mit HTML verwenden.

#### CSS einbinden und verwenden

##### Variante 1 - in eine extra Datei auslagern und einbinden

Hierzu wird eine neue Datei mit der Dateiendung `.css` angelegt. Anschließend wird diese über einen `<link>` HTML-Tag (für eine verlinkte Einbindung) extern im Kopf der HTML-Seite eingebunden.

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="utf-8">
    <title>Seitentitel</title>
    <link href="style.css" rel="stylesheet" type="text/css">
</head>
<body>

</body>
</html>
```

| Tag      | Attribut | Erklärung                                         |
| -------- | -------- | ------------------------------------------------- |
| `<link>` | `href`   | definiert den Pfad zur eingebundenen Datei        |
|          | `rel`    | bestimmt die Beziehung *(relationship)* zur Datei |
|          | `type`   | definiert den Typ der eingebundenen Datei         |

##### Variante 2 - direkt in die HTML-Datei schreiben

Hierzu wird im HTML-Code über den `<style>`  HTML-Tag der CSS-Code direkt intern eingebunden. Meistens wird der Tag im Kopfbereich eingebunden, kann allerdings an jeder Position des HTML-Codes stehen.

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="utf-8">
    <title>Seitentitel</title>
    <style type="text/css">
    </style>
</head>
<body>

</body>
</html>
```

| Tag       | Attribut | Erklärung                                  |
| --------- | -------- | ------------------------------------------ |
| `<style>` | `type`   | definiert den Typ für den verwendeten Code |

#### CSS Aufbau

```css
selektor {
   eigenschaft: wert;
}
```

```css
body {
   background: green;
}
```

##### CSS-Selektoren

Damit die Formateigenschaften auf ein Element angewendet werden können, muss definiert werden, welche Elemente angesprochen werden. Dies geschieht über **Selektoren**.  Als CSS Selektoren bezeichnet man die Teile einer CSS-Regel, die vor dem Abschnitt aus geschweiften Klammern stehen. 

Die wichtigsten Selektoren sind die **Element**e, **Klassen** und **ID's**

###### Element-Selektoren

Der Element- bzw. Typselektor besteht aus dem **Namen des Elements**, das angesprochen werden soll. Mit diesem Selektor werden alle Elemente eines Typs angesprochen.

```html
<style type="text/css">
 p {
   color: red;
 }
</style>
```

###### Klassen-Selektoren

Ein Klassenselektor spricht Elemente an, die einer **bestimmten Klasse** zugehörend sind. Im HTML-Code kann jeder Tag mit einer Klasse - über das Attribut `class`  - versehen werden. Im CSS wird dieser über einen Punkt (`.`)  vor der Klasse angesprochen.

```html
<body>
  <p>Dies ist eine Zeile</p>
  <p class="hinweis">Dies ist ein Hinweis</p>
  <p>Dies ist eine weitere Zeile</p>
  <p class="hinweis">Dies ist ein weiterer Hinweis</p>
</body>
```

> Jetzt werden ausschließlich nur  `p`-Elemente mit der Klasse `hinweis` mit roter Schriftfarbe dargestellt. Die `<p>`-Tags ohne `class="hinweis"` bleiben unverändert.

###### ID-Selektoren

 Mit dem ID-Selektor kann ein Element angesprochen werden, dem eine **ID zugeordnet** wurde. Im HTML-Code kann jeder Tag mit einer ID - über das Attribut `id`  - versehen werden. Im CSS wird dieser über eine Raute (`#`) vor der ID angesprochen.

 ```html
 <body>
   <ul id="navigation">
     <li>Menüpunkt 1</li>
     <li>Menüpunkt 2</li>
     <li>Menüpunkt 3</li>
   </ul>
 </body>
 ```

```html
 <style type="text/css">
  #navigation {
    margin-left: 20px;
  }
 </style>
```


#### HTML DOM

##### Aufbau Tag

Ein Tag *(HTML-Element)* steht grundsätzlich mit seiner Tag-Bezeichnung in spitzen Klammern. Tags können um **Attribute** weiter spezialisiert werden. Die gängigen Attribute sind Style-Zuweisungen für CSS mittels *Klassen* oder *ID's*. Bis auf wenige Ausnahmen wie der  `<img>` Tag, wird jeder Tag wieder mit einem Backslash und der Bezeichnung in spitzen Klammern beendet.

##### HTML DOM

Der HTML DOM ist eine Modellierung der HTML-Webseite. Visuell wird damit die Struktur und Hierarchien des HTML-Dokuments dargestellt. 

Im Eigentlichen dient dieser zur Manipulation von HTML-Elementen mittels Programme und Skripte. Die Darstellung als Modell hilft allerdings im Layout, um einzelne Hierarchien zu durchblicken.

##### Box Prinzip

Im HTML kommt grundsätzlich ein „Box-Prinzip“ zum Einsatz. Die meisten dargestellten Inhalte wie **Kopfzeile**, **Navigation**, **Seiteninhalt** und **Fußzeile** sind jeweils einzelne Einheiten, also für sich separierte Bereiche.

###### div-Tag

Für die Trennung und Einteilung in eigene Bereich kommt der `<div>` Tag zum Einsatz. Der Tag wird um verschiedene HTML-Elemente wie Text, Grafiken, Tabellen geschachtelt, die eine Einheit darstellen sollen.

Damit im HTML nicht grundsätzlich alle Elemente ein bestimmtes Layout mittels CSS erhalten sollen, sondern speziell für den gewünschten Bereich wird der Tag um eine Klasse oder ID erweitert und ist damit in CSS ansteuerbar.  

```html
<body>
    <h1>Allgemeines Blockelement</h1>

    <div class="einfuehrung">
      <h2>Listenüberschrift</h2>

      <ul>
        <li>Listenpunkt 1</li>
        <li>Listenpunkt 2</li>
      </ul>
    </div>
</body>
```

So sollen auf sämtlichen Seiten nun zum Beispiel die Überschrift in einem Einführungsabschnitt eine andere Farbe erhalten. Damit nun nicht grundsätzlich die Überschriften die im Quelltext vorkommen diese besondere Eigenschaft erhalten, wird diese in CSS spezifisch angesprochen:

```css
.einfuehrung h2 {
    color: #cccccc;
}
```

###### Layout-Tags in HTML5

In Vergangenheit mussten also für die zu vor genannten Layout Bereiche wie Kopfzeile, Navigation oder Fußzeile jeweils eigene `div`-Tags mit einer CSS-Zuweisung definiert werden. Seit HTML5 gibt es zahlreiche neue Tags, die speziell für diesen Einsatz entwickelt wurden. So können Tags wie `<header>` für die Kopfzeile, `<nav>` für Navigationsbereiche oder `<footer>` für Fußzeilen genutzt werden.

#### Tabellen

Eine Tabelle ist eine geordnete Kombination von Daten oder Texte. Die Inhalte werden in **Zeilen** (waagerecht) und **Spalten** (senkrecht) angeordnet.

Im Normalfall besteht eine Tabelle aus Tabellenzeilen, in der wiederum Tabellenzellen gegliedert werden.

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="utf-8">
    <title>Seitentitel</title>
</head>
<body>
    <table>
        <tr>
            <td>Inhalt</td>
        </tr>
    </table>
</body>
</html>
```

| Tag       | Erklärung                                                    |
| --------- | ------------------------------------------------------------ |
| `<table>` | leitet eine Tabelle ein (table = Tabelle)                    |
| `<th>`    | leitet eine Kopfzelle ein (th = table header = Tabellenkopf) |
| `<tr>`    | leitet eine neue Tabellenzeile ein (tr = table row = Tabellenzeile) |
| `<td>`    | eine normale Datenzelle (td = table data = Tabellendaten)    |

## Entwicklung mit **Vue**

Ein Rückblick auf die letzten Jahrzehnte des Internets bringen ein Fazit: Das Web und die Webentwicklung schreiten immer weiter voran. Zumal sich eine Richtung kristallisiert. Immer größer werdende JavaScript Anwendungen bringen einen zentralen Markt für neue Lösungen: JavaScript Frameworks für das Handling komplexer Webprojekte.

### Entstehung von Vue

Vue wurde von _Evan You_ erfunden, der vorher Mitarbeiter bei Google war. Dort arbeitete er zusammen mit seinem Team an verschiedene Software-Prototypen. Hauptsächlich wurden diese über das hauseigene Konkurrenz-Framework _AngularJS_ realisiert.

Während seiner Arbeit lernte er zwar das Framework zu schätzen, aber auch viele Nachteile fielen in's Auge. So sei AngularJS zwar mächtig und reich an Funktionalitäten, aber der Fokus für die einfache, schnelle und zielorientierte Entwicklung fehlt vollkommen.

Demnach begann er ein eigenes Nebenprojekt. _Vue_ war damit geboren.

### Was ist Vue?

[basiert auf Inhalte von https://www.hosteurope.de/blog/einfuehrung-in-vue-js-was-steckt-wirklich-hinter-dem-progressiven-framework/]

Vue bezeichnet sich selbst als **Progressive Framework **, also als "fortschrittliches Framework". Vue passt sich damit an die Komplexität der eigentlichen Codebasis an. Das Wichtigste an Vue ist nebenbei aber auch der **Virtual DOM** und das **Deklarative Rendering bei Single File Components**. Es zählt im Übrigen zu den **Single-Page-Applications** (kurz SPA). Damit sind Anwendungen gemeint, die grundsätzlich nur **einer einzigen HTML-Datei** bestehen und die jeweiligen Inhalte (Komponente) dynamisch nachlädt.

#### Virtual DOM

Mit _virtuellen DOM_ ist ein abstraktes Duplikat des eigentlichen DOMs gemeint. Ein intelligenter Algorithmus vergleicht im Anschluss die Unterschiede in einem Zug im [tatsächlich gerendertem DOM](https://t3n.de/news/eigentlich-virtuelles-dom-858160/).

#### Single File Components

Vue.js verwendet [Single File Components](https://vuejs.org/v2/guide/single-file-components.html#ad). Durch ein "dynamisches Bundling" ist es möglich, HTML, JavaScript und CSS in seperate Dateien abzulegen — generell werden alle drei Bestandteile aber in eine Datei kompiliert. Kleine Komponenten haben den Vorteil, testbar, wartbar und leicht erweiterbar zu sein. Diese Komponenten folgen daher dem Prinzip des _Separation of Concerns_. Dieses Prinzip bedeutet, dass man Zuständigkeiten strikt voneinander trennt. Eine einzelne Komponente erfüllt genau eine Aufgabe, nicht mehr und nicht weniger. Dadurch kann gewährleistet werden, dass die Komponente universell einsetzbar ist.

### Template

Vue.js lässt einem generell viel Gestaltungsfreiraum. Die einfachste Variante, um ein Databinding mit dem Script herzustellen, ist die “Mustache” Syntax, die man bereits von [Handlebars](https://handlebarsjs.com/) kennt:

```
<p>{{ greeting }} World!</p>
```

In den Platzhalter wird automatisch von Vue.js der Wert `hello` des Data-Attributs eingesetzt. Ändert man im Script den Wert von `greeting`, passt sich auch das Template automatisch an. Dafür muss der Entwickler nicht mehr den Selektor anfragen und den Wert spezifisch ändern.

Außerdem stehen weitere Schlüsselwörter, Funktionen zur Verfügung, unter anderem:

- `v-if` / `v-else`
- `v-show`
- `v-once`
- `v-html`
- `v-text`

Auch Eventhandler können direkt an das HTML Tag hinzugefügt werden, zum Beispiel:

- `@click`
- `@click.prevent` für automatisches Aufrufen von`event.preventDefault()`
- `@click.stop` für automatisches Aufrufen von `event.stopPropagation()`

Um dynamische Werte an das Tag zu binden, benutzt man ein Shorthand mit einem Doppelpunkt als Prefix, zum Beispiel:

- `v-bind:href`
- `v-bind:src`
- `:href` (mit Shorthand)
- `:src` (mit Shorthand)

## DVB **Vue-Webprojekt**

Das DVB-Webprojekt vereint verschiedene Technologien. Zu einem natürlich **Vue** selbst, aber auch **Node.js**, **JSON** und selbstverständlich **HTML5/CSS** und **JavaScript**. 

?> Node.js ist ein eine [serverseitige](https://de.wikipedia.org/wiki/Client-Server-Modell) Plattform für Webapplikationen. Damit lassen sich u. a. JavaScript Projekte einfach über mittels verschiedene Module verwalten und agiert als eine Projektumgebung. Jedes Node.js-Projekt hat dabei eine eigene `package.json`-Datei, in der alle verwendeten Module mit ihrer Versionierung hinterlegt sind. Aber auch Angaben wie Name, Autor und Version des eigenen Projektes selbst.

Wir nutzen für unser Webprojekt die Node.js-Umgebung. Leider lässt diese sich schwer via den Online-Compiler _repl.it_ verwenden. Aus diesem Grund nutzen wir alternativ die **[CodeSandbox](https://codesandbox.io/s)**. Dort stellen wir ein Projekt-Grundgerüst zum Mitentwickeln bereit. 

### Node.js Module

Unser Projekt nutzt nachfolgend die Module.

| Modul        | Version | Verwendung                                     |
| :----------- | :------ | ---------------------------------------------- |
| `vue`        | 2.5.22  | Vue Framework                                  |
| `vue-i18n`   | 8.11.2  | Internationalisierung/Mehrsprachigkeit der App |
| `vue-router` | 3.0.6   | Deklaration von internen URL-Routen            |
| `vuex`       | 3.1.1   | Zentralisierter Datastore                      |
| `axios`      | 0.19.0  | Verwendung von APIs                            |

Definiert wurden diese in der `package.json`-Datei im Absatz:

```
  "dependencies": {
    "vue": "^2.5.22",
    "vue-router": "^3.0.6",
    "vue-i18n": "^8.11.2",
    "vuex": "^3.1.1",
    "axios": "^0.19.0"
  },
```

### Projektstruktur

| Verzeichnis/Dateien | Verwendung                          |
| ------------------- | ----------------------------------- |
| `public`            | Hinterlegen der Style-Ressourcen    |
| – `css`             | CSS-Dateien                         |
| – `favicon.ico`     | Bild-Datei für Lesezeichenliste     |
| – `index.html`      | **Hauptdatei**                      |
| `src`               | Hinterlegen der Quell-Dateien       |
| – `assets`          | Bilder                              |
| – – `logo.png`      | Vue-Logo als Beispiel |
| – `components`      | Vue-Komponente (Ansichten)       |
| – – `Home.vue`      | Komponente Start                 |
| – – `Imprint.vue`   | Komponente Imprint |
| – `router`          | Hinterlegen der Komponenten-Routen |
| – – `index.js`   | Definition der Routen |
| –`App.vue`   | Haupt-Vue-Datei |
| – `main.js`   | Haupt-Javascript mit Vue-Implementation |
| `package.json`   | Projektidentität |

### VVO-Schnittstelle

!> Die Informationen wurden von _Kilian Koeltzsch_ zusammengetragen. Probs to you! <3

Die **VVO Web-Schnittstelle** lässt sich via JSON ansprechen. Die Basis-URL lautet `https://webapi.vvo-online.de`.  Für die JSON-Anfrage muss am Ende der Anfrage jeweils der Parameter `?format=json` angehängt werden. Nachfolgend sind die verschiedene zur Verfügung stehenden Funktionen notiert.

#### PointFinder

!> Findet Haltestellen zu einer Suchanfrage

##### Anfrage

`https://webapi.vvo-online.de/tr/pointfinder?format=json`

JSON body:

| Name        | Type   | Description                     | Required |
| ----------- | ------ | ------------------------------- | -------- |
| `query`     | String | Search query                    | Yes      |
| `limit`     | Int    | Maximum number of results       | No       |
| `stopsOnly` | Bool   | Only search for stops if `true` | No       |

or

| Name            | Type   | Description                                    | Required |
| --------------- | ------ | ---------------------------------------------- | -------- |
| `query`         | String | `coord:[right]:[up]` in GK4 coordinates        | Yes      |
| `limit`         | Int    | Maximum number of results                      | No       |
| `assignedstops` | Bool   | Include stops assigned to coordinate if `true` | No       |

`[right]` and `[up]` are placeholders for the actual coordinates in this example.

##### Antwort (Exemplarisch)

```js
{
  "PointStatus": "List",
  "Status": {
    "Code": "Ok"
  },
  "Points": [
    "33000742|||Helmholtzstraße|5655904|4621157|0||",
    "36030083||Chemnitz|Helmholtzstr|5635837|4566835|0||",
    "9022020||Bonn|Helmholtzstraße|0|0|0||"
  ],
  "ExpirationTime": "\/Date(1487859556456+0100)\/"
}
```

Be aware that the elements of the `Points` array can take different forms with different types. If doing a PointFinder request for a coordinate, the first element will look like the following for example `coord:4621020:504065:NAV4:Nöthnitzer Straße 46|c||Nöthnitzer Straße 46|5655935|4621020|0||`.

Any info on the format of the strings contained within `Points` would be much appreciated.


#### Departure Monitor

!> Anzeige der kommenden Abfahrten zu einer Haltestelle

##### Anfrage

`https://webapi.vvo-online.de/dm?format=json`

JSON body:

| Name               | Type          | Description                              | Required |
| ------------------ | ------------- | ---------------------------------------- | -------- |
| `stopid`           | String        | ID of the stop                           | Yes      |
| `limit`            | Int           | Maximum number of results                | No       |
| `time`             | String        | ISO8601 timestamp, e.g. `2017-02-22T15:40:26Z` | No       |
| `isarrival`        | Bool          | Is the time specified above supposed to be interpreted as arrival or departure time? | No       |
| `shorttermchanges` | Bool          | unknown in this context                  | No       |
| `mot`              | Array[String] | Allowed modes of transport, see below    | No       |

Currently accepted modes of transport are `Tram`, `CityBus`, `IntercityBus`, `SuburbanRailway`, `Train`, `Cableway`, `Ferry`, `HailedSharedTaxi`.

##### Antwort (Exemplarisch)

```js
{
  "Name": "Hauptbahnhof",
  "Status": {
    "Code": "Ok"
  },
  "Place": "Dresden",
  "ExpirationTime": "\/Date(1487778279147+0100)\/",
  "Departures": [
    {
      "Id": "65597047",
      "LineName": "3",
      "Direction": "Wilder Mann",
      "Platform": {
        "Name": "3",
        "Type": "Platform"
      },
      "Mot": "Tram",
      "RealTime": "\/Date(1487778230000+0100)\/",
      "ScheduledTime": "\/Date(1487778060000+0100)\/",
      "State": "Delayed",
      "RouteChanges": [
        "509223"
      ],
      "Diva": {
        "Number": "11003",
        "Network": "voe"
      }
    },
    {
      "Id": "65598309",
      "LineName": "8",
      "Direction": "Südvorstadt",
      "Platform": {
        "Name": "4",
        "Type": "Platform"
      },
      "Mot": "Tram",
      "RealTime": "\/Date(1487778356000+0100)\/",
      "ScheduledTime": "\/Date(1487778300000+0100)\/",
      "State": "InTime",
      "Diva": {
        "Number": "11008",
        "Network": "voe"
      }
    }
  ]
}
```


### Trip Details

Infos über Haltestellen zu einem Trip

##### Anfrage

`https://webapi.vvo-online.de/dm/trip?format=json`

JSON Body:

| Name	    | Type	    | Description	                                                    | Required |
| --------- | --------- | ----------------------------------------------------------------- | -------- |
| `tripid`  | String	| The "id" received from the departure monitor (Departures\[\*\].Id).	| Yes      |
| `time`    | String	| The current time as unix timestamp plus timezone. Has to be in the future. Most likely from a departure monitor response (Departures\[\*\].RealTime / Departures\[\*\].ScheduledTime). | Yes |
| `stopid`  | String	| ID of a stop in the route. This stop will be marked with Position=Current in the response. | Yes |
| `mapdata` | Bool	    | Unknown. Seems to have no effect.	                                | No       |

##### Antwort (Exemplarisch)
```
{
  "Stops": [
    ...
    {
      "Id": "33000076",
      "Place": "Dresden",
      "Name": "Laibacher Straße",
      "Position": "Previous",
      "Platform": {
        "Name": "2",
        "Type": "Platform"
      },
      "Time": "\/Date(1512563021000+0100)\/"
    },
    {
      "Id": "33000077",
      "Place": "Dresden",
      "Name": "Großglocknerstraße",
      "Position": "Current",
      "Platform": {
        "Name": "2",
        "Type": "Platform"
      },
      "Time": "\/Date(1512563081000+0100)\/"
    },
    {
      "Id": "33000078",
      "Place": "Dresden",
      "Name": "Friedhof Leuben",
      "Position": "Next",
      "Platform": {
        "Name": "2",
        "Type": "Platform"
      },
      "Time": "\/Date(1512563141000+0100)\/"
    },
    ...
  ],
  "Status": {
    "Code": "Ok"
  },
  "ExpirationTime": "\/Date(1512565171371+0100)\/"
}
```


### Query a Trip

!> Infos zu einem Trip von Punkt A zu Punkt B 

Beispiel "Hauptbahnhof" (stopid 33000028) zur Haltestelle "Bahnhof Neustadt" (stopid 33000016).

##### Anfrage

`https://webapi.vvo-online.de/tr/trips?format=json`

JSON body

| Name               | Type        | Description       | Required |
| ------------------ | ----------- | ----------------- | -------- |
| `origin`           | String      | stopid of start station | yes |
| `destination`      | String      | stopid of destination station | yes |
| `shorttermchanges` | Bool        | unknown           | no (missing behaves like `shorttermchanges = false`) |
| `time`             | String      | ISO8601 timestamp | no  |
| `isarrivaltime`    | Bool        | is `time` arrival or departure | no |

##### Antwort (Exemplarisch)

```json
{
    "Routes": [
        ...
        {
            "Duration": 11,
            "FareZoneDestination": 10,
            "FareZoneOrigin": 10,
            "Interchanges": 0,
            "MapData": [
                "Tram|5657496|4621684|5657555|4621712|5657572|4621722|5657589|4621733|5657611|4621746|5657637|4621762|5657694|4621796|5657694|4621796|5657700|4621800|5657729|4621819|5657795|4621859|5657861|4621902|5657888|4621922|5657930|4621954|5657978|4621990|5657978|4621990|5658017|4622019|5658176|4622138|5658240|4622191|5658279|4622224|5658347|4622282|5658358|4622291|5658377|4622302|5658414|4622319|5658476|4622350|5658551|4622387|5658551|4622387|5658574|4622398|5658588|4622406|5658595|4622411|5658607|4622421|5658621|4622432|5658628|4622440|5658629|4622441|5658638|4622450|5658661|4622474|5658682|4622494|5658692|4622502|5658702|4622509|5658765|4622541|5658816|4622567|5658852|4622582|5658870|4622587|5658888|4622592|5658901|4622595|5658937|4622602|5658957|4622607|5658957|4622607|5658966|4622609|5658990|4622613|5659010|4622615|5659021|4622615|5659035|4622614|5659058|4622612|5659091|4622606|5659388|4622527|5659435|4622516|5659441|4622514|5659473|4622506|5659512|4622508|5659520|4622508|5659556|4622511|5659556|4622511|5659562|4622512|5659581|4622513|5659603|4622512|5659946|4622487|5659981|4622486|5660008|4622484|5660032|4622487|5660053|4622494|5660065|4622499|5660090|4622515|5660123|4622534|5660124|4622534|5660124|4622534|5660134|4622541|5660148|4622549|5660244|4622401|5660271|4622315|5660278|4622254|5660285|4622217|5660291|4622151|"
            ],
            "MapPdfId": "VVO_5A2B062D3",
            "MotChain": [
                {
                    "Changes": [
                        "510690"
                    ],
                    "Direction": " Btf Trachenberge",
                    "Diva": {
                        "Network": "voe",
                        "Number": "11003"
                    },
                    "Name": "3",
                    "Type": "Tram"
                }
            ],
            "PartialRoutes": [
                {
                    "Duration": 11,
                    "MapDataIndex": 0,
                    "Mot": {
                        "Changes": [
                            "510690"
                        ],
                        "Direction": " Btf Trachenberge",
                        "Diva": {
                            "Network": "voe",
                            "Number": "11003"
                        },
                        "Name": "3",
                        "Type": "Tram"
                    },
                    "PartialRouteId": 0,
                    "RegularStops": [
                        {
                            "ArrivalTime": "/Date(1512769800000-0000)/",
                            "DataId": "33000028",
                            "DepartureTime": "/Date(1512769800000-0000)/",
                            "Latitude": 5657497,
                            "Longitude": 4621685,
                            "MapPdfId": "VVO_5A2B062D4",
                            "Name": "Hauptbahnhof",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "3",
                                "Type": "Railtrack"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512769860000-0000)/",
                            "DataId": "33000032",
                            "DepartureTime": "/Date(1512769860000-0000)/",
                            "Latitude": 5657693,
                            "Longitude": 4621797,
                            "Name": "Hauptbahnhof Nord",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "1",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512769920000-0000)/",
                            "DataId": "33000029",
                            "DepartureTime": "/Date(1512769920000-0000)/",
                            "Latitude": 5657981,
                            "Longitude": 4621985,
                            "Name": "Walpurgisstraße",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "1",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512770040000-0000)/",
                            "DataId": "33000005",
                            "DepartureTime": "/Date(1512770040000-0000)/",
                            "Latitude": 5658549,
                            "Longitude": 4622390,
                            "Name": "Pirnaischer Platz",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "4",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512770100000-0000)/",
                            "DataId": "33000015",
                            "DepartureTime": "/Date(1512770100000-0000)/",
                            "Latitude": 5658956,
                            "Longitude": 4622609,
                            "Name": "Synagoge",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "2",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512770220000-0000)/",
                            "DataId": "33000014",
                            "DepartureTime": "/Date(1512770220000-0000)/",
                            "Latitude": 5659556,
                            "Longitude": 4622513,
                            "Name": "Carolaplatz",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "4",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512770340000-0000)/",
                            "DataId": "33000013",
                            "DepartureTime": "/Date(1512770340000-0000)/",
                            "Latitude": 5660122,
                            "Longitude": 4622537,
                            "Name": "Albertplatz",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "2",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        },
                        {
                            "ArrivalTime": "/Date(1512770460000-0000)/",
                            "DataId": "33000016",
                            "DepartureTime": "/Date(1512770460000-0000)/",
                            "Latitude": 5660290,
                            "Longitude": 4622151,
                            "MapPdfId": "VVO_5A2B062D5",
                            "Name": "Bahnhof Neustadt",
                            "Place": "Dresden",
                            "Platform": {
                                "Name": "2",
                                "Type": "Platform"
                            },
                            "Type": "Stop"
                        }
                    ],
                    "Shift": "None"
                }
            ],
            "Price": "2,30",
            "PriceLevel": 1,
            "RouteId": 1
        },
        ...
    ],
    "SessionId": "367417461:efa4",
    "Status": {
        "Code": "Ok"
    }
}
```


#### Route Changes

!> Infos zu Fahrplanänderungen

##### Anfrage

`https://webapi.vvo-online.de/rc?format=json`

JSON body

| Name        | Type        | Description    | Required |
| ----------- | ----------- | -------------- | -------- |
| `shortterm` | Bool        | unknown. I diffed the output with and without -> no diff | no        |

##### Antwort (Exemplarisch)

```json
{
    "Changes": [
        ...
        {
            "Description": "<p><DIV ></DIV>\n<H2>Beschreibung</H2>\n<P><STRONG>Buslinie 79:</STRONG><BR>Umleitung <FONT color=#ff0000>nur in Richtung&nbsp;Overbeckstraße</FONT> zwischen den Haltestellen&nbsp;Rethelstraße und&nbsp;Mengsstraße über den Fahrweg <U>Rethelstraße - Werftstraße</U>.</P>\n<H2>Haltestellenanpassungen</H2>\n<UL>\n<LI>Die Haltestellen <STRONG>Kaditzer Straße</STRONG> und <STRONG>Thäterstraße</STRONG>&nbsp;werden in die <U>Rethelstraße</U> verlegt.</LI></UL></p>",
            "Id": "511595",
            "LineIds": [
                "428296"
            ],
            "PublishDate": "/Date(1512400560000+0100)/",
            "Title": "Dresden - Mengsstraße, Vollsperrung wegen Asphaltarbeiten",
            "Type": "Scheduled",
            "ValidityPeriods": [
                {
                    "Begin": "/Date(1512529200000+0100)/",
                    "End": "/Date(1512788400000+0100)/"
                }
            ]
        },
        ...
    ],
    "Status": {
        "Code": "Ok"
    }
}
```

(sometimes they come back: `<font color="#abc" />`)

