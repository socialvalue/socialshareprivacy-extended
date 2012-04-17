
 jquery.socialshareprivacy.js | 2 Klicks fuer mehr Datenschutz

 http://www.heise.de/extras/socialshareprivacy/
 http://www.heise.de/ct/artikel/2-Klicks-fuer-mehr-Datenschutz-1333879.html
 
 Copyright (c) 2011 Hilko Holweg, Sebastian Hilbig, Nicolas Heiringhoff, Juergen Schmidt,
 Heise Zeitschriften Verlag GmbH & Co. KG, http://www.heise.de

 is released under the MIT License http://www.opensource.org/licenses/mit-license.php

 Spread the word, link to us if you can.

 jquery.socialshareprivacy-xl.js | Erweiterung für Xing und LinkedIn

 http://www.illusions-schmiede.com/Tools/Socialshareprivacy-XL

 Copyright (c) 2012 David Sann
 Illusions-Schmiede Gmbh http://www.illusions-schmiede.com

 is released under the MIT License http://www.opensource.org/licenses/mit-license.php


1) 	Einleitung

2) 	Zusatzfunktionen
2.1)	Unterstützung von Xing und LinkedIn
2.2)	Benutzerdefinierte Include-Codes

3) 	Installation


1) Einleitung
--------------

Socialshareprivacy-XL ist eine Erweiterung des JavaScript Plugins Socialshareprivacy des Heise Verlags.
Zur Funktion der Erweiterung ist die beinhaltete Version des Socialshareprivacy Plugins dringend notwendig.

Folgende Funktionen wurden zusätzlich mit eingebunden:

2) Zusatzfunktionen
--------------------

2.1) Unterstützung von Xing und LinkedIn

Socialshareprivacy wurde um die Share-Buttons von Xing und LinkedIn erweitert. Die Einbindung und Konfiguration funktioniert
analog zu den bisher unterstützen Buttons von facebook, Twitter und Google+.

2.2) Benutzerdefinierte Include-Codes

Die Anbieter der Share-Buttons bieten meist auf ihren Seiten mehrere Möglichkeiten diese auf der eigenen Webseite einzubinden
(z.B. mit oder ohne Counter, etc.). Über den Parameter share_btn_code können Sie ihren individuell generierten Code in das 
Socialshareprivacy Plugin einbinden. Wird der Parameter nicht verwendet, oder ist er leer, so wird der Standard-Code verwendet.

3) Installation und Konfiguration
----------------

Folgen sie bitte den Anweisungen in der index.html (Im Paket enthalten) zu der Installation des Plugins von Heise.
Um die Funktionen von Socialshareprivy-XL nutzen zu können, ersetzen Sie einfach die folgende Zeilen:

- die Einbindug der js-Datei:

<script type="text/javascript" src="jquery.socialshareprivacy.js"></script>

wird ersetzt durch 

<script type="text/javascript" src="jquery.socialshareprivacy-xl-min.js"></script>
oder
<script type="text/javascript" src="jquery.socialshareprivacy-xl.js"></script>

(wir empfehlen die minimierte Version einzubinden, da dadurch die Ladezeit stark verkürzt wird)
Ebenfalls liegt dieser Version die minimierte Version von jQuery 1.7.1 bei, welche anstatt der nicht-minimierten Version 1.6.4 verwendet werden kann.

- die Angabe der CSS-Datei:

'css_path' : '/style/plugins/socialshareprivacy.css'

wird ersetzt durch

'css_path' : '/style/plugins/socialshareprivacy-xl.css'


Mit dem Parameter share_btn_code kann für jeden einzelnen Button ein individueller Einbinde-Code angegeben werden.

Bsp:

$('#socialshareprivacy').socialSharePrivacy({
    services : {
        facebook : {
            'perma_option'  : 'off',
            'share_btn_code' : '[Ihr individuell erstellter Code]'
        }
    }
});























