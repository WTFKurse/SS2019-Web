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
			![Patrik Phan](_images/teacher_patrik.jpg 'Patrik Phan')
		</div>
		<div class="contact">
			<h4>Patrik Phan</h4>
			patrik@wtfkurse.de
		</div>
	</div>
	<div class="teacher">
		<div class="avatar">
			![Kevin Schmid](_images/teacher_kevin.jpg 'Kevin Schmid')
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
>
> ###### ID-Selektoren
>
> Mit dem ID-Selektor kann ein Element angesprochen werden, dem eine **ID zugeordnet** wurde. Im HTML-Code kann jeder Tag mit einer ID - über das Attribut `id`  - versehen werden. Im CSS wird dieser über eine Raute (`#`) vor der ID angesprochen.
>
> ```html
> <body>
>   <ul id="navigation">
>     <li>Menüpunkt 1</li>
>     <li>Menüpunkt 2</li>
>     <li>Menüpunkt 3</li>
>   </ul>
> </body>
> ```
>
> ```html
> <style type="text/css">
>  #navigation {
>    margin-left: 20px;
>  }
> </style>
> ```
>
> 

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

| Tag     | Erklärung                                                    |
| ------- | ------------------------------------------------------------ |
|`<table>` | leitet eine Tabelle ein (table = Tabelle)                    |
| `<th>`    | leitet eine Kopfzelle ein (th = table header = Tabellenkopf) |
| `<tr>`    | leitet eine neue Tabellenzeile ein (tr = table row = Tabellenzeile) |
| `<td>`    | eine normale Datenzelle (td = table data = Tabellendaten)    |
