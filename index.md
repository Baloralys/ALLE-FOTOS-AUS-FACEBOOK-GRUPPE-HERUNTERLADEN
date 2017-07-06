# ALLE-FOTOS-AUS-FACEBOOK-GRUPPE-HERUNTERLADEN
Mit diesem Javascript könnt ihr die Fotos aus den einzelnen Alben einer Facebookgruppe herunterladen und müsst nicht jedes einzelnd anklicken.

## ANLEITUNG:
Hier wird genau beschrieben, wie du alle Fotos aus einem Facebook-Gruppen Fotoalbum downloaden kannst.

1. Klicke bei der Facebook-Gruppe auf FOTOS > ALBUM AUSWÄHLEN

2. Scrolle bis ganz nach unten, damit die Fotos vollständig geladen werden, da sonst nicht alle Fotos geladen werden

3. Drücke jetzt (gleichzeitig)

Tastenkombination  | Browser
------------- | -------------
**STRG + SHIFT + J**  | Google Chrome

Es wird sich ein Fenster mit einem Eingabebereich öffnen. 
Bei Google Chrome Browser muss man zusätzlich zuerst auf CONSOLE klicken.

###### Für Facebook-Gruppen folgenden Code kopieren und einfügen. Danach auf Enter drücken:
```javascript
javascript:var items = document.getElementsByClassName('_53s fbPhotoCurationControlWrapper fbPhotoStarGridElement fbPhotoStarGridNonStarred _53s fbPhotoCurationControlWrapper');var divsToAppend = ""; for (var i = 0; i < items.length; i++){ divsToAppend += '<a href="'+ items[i].getAttribute("data-starred-src") +'" class="dlpic" download="">Download</a>'; };document.body.innerHTML = divsToAppend; var inputs = document.getElementsByClassName('dlpic'); for(var i=0; i<inputs.length;i++) { inputs[i].click() };
```

***

**Hinweis: Achte auch nach dem kopieren und einfügen bitte darauf, dass "javascript" ebenfalls eingefügt wurde. Und beachte das Download-Verzeichnis beim Google Chrome Browser, sinnvoll wäre es einen extra Ordner anzulegen und den Download dorthin zu verweisen.**


> Bitte beachten: Je nach Anzahl der Fotos und Geschwindigkeit des Rechners kann das eine ganze Weile dauern. Man muss nur etwas Geduld haben.