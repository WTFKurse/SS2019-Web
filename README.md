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
