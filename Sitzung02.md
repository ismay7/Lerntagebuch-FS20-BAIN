# Sitzung 2

Datum: 03.04.2020

### Thema: Funktion und Aufbau von Bibliothekssystemen

Das grosse Thema der heutigen Sitzung (03.04.2020) ist die Funktion und der Aufbau von Bibliothekssystemen. 

#### Datenvisualisierung

Bevor wir nun aber in das Hauptthema der Sitzung vordringen, haben wir ein sehr aktuelles Thema vorneweg angeschaut, nämlich Datenvisualisierungen und zwar zu folgendem: 

It will go down in history – CORONA, das Virus [SARS-CoV-2](https://de.wikipedia.org/wiki/SARS-CoV-2), das mit Lockdowns in fast allen Ländern die Welt lahm legt und uns vor die Bildschirme zuhause ins WebEx Meeting verlegt hat.

Wir besprechen also als Warm-Up gewissermassen erst die aktuellen und populärsten Datenvisualisierungen zum Virus, wie sie beispielsweise hier zu finden sind:

- [Tagesspiegel](https://interaktiv.tagesspiegel.de/lab/die-globale-verbreitung-des-coronavirus-im-zeitverlauf/)
- [Johns Hopkins University](https://coronavirus.jhu.edu/map.html)
- [NCOV](https://ncov2019.live/data)
- [Bundesamt für Gesundeheit Schweiz (BAG)](https://covid-19-schweiz.bagapps.ch/de-1.html)

Ich persönlich kann mich der Meinung der Mehrzahl der Studierenden anschliessen, dass die Johns Hopkins Universität eine sehr ausgereifte, interaktive Statistik-Karte geschaffen hat. Wenn es um die Zahlen und sonstige Informationen zum Thema geht, bin ich jedoch eher konservativ und höre mir an, was unser BAG dazu meldet. Schliesslich gehe ich davon aus, dass dort die Zahlen und Fakten aus erster “Messungshand” stammen und sehr aktuell sind. Allerdings ist es ja bei diesem Virus ohnehin so, dass nicht alle positiven Fälle in die Statistik kommen, da nur Menschen mit Symptomen überhaupt getestet werden und viele junge Menschen, das Virus zwar tragen können, aber gar nichts davon merken. Insofern fragt man sich, wie die Statistik überhaupt gelesen werden muss und wie aussagekräftig das Ganze ist.

![](Sitzung02.assets/corona-28-6.png)

Screenshot aktualisiert vom 28.6.20 ([Johns Hopkins University](https://coronavirus.jhu.edu/map.html))



### Installation und Konfiguration von Koha

[Koha](https://koha-community.org/) ist ein webbasiertes integriertes Bibliothekssystem, das weltweit durch viele öffentliche Bibliotheken und Archive zum Einsatz kommt. Die Software ist komplett open-source. Es ist besonders auf Skalierbarkeit ausgelegt und bedient sich einer SQL-Datenbankanbindung (vorzugsweise MySQL oder MariaDB). Koha verfügt über die üblichen Funktionen integrierter  Bibliothekssysteme wie die Verwaltung von Umläufen und Ausleihen,  Bestandsverwaltung und Unterstützung für Periodika wie Zeitschriften und Zeitungen ([Wikipedia, 2020](https://de.wikipedia.org/wiki/Koha_(Bibliothekssoftware))). 

Wie bereits erwähnt, lief die Azure VM bei mir nur sehr stotternd und war teilweise einfach nicht so richtig zu gebrauchen. Deshalb entschied ich mich, obwohl bereits auf dem Remote Desktop installiert, Koha 19.11 nochmals in einer Ubuntu-VM auf meinem System zu installieren (via [GNOME Boxes](https://covid-19-schweiz.bagapps.ch/de-1.html)). Ich habe dazu das aktuelle Ubuntu 20.04 LTS verwendet und bin gewöhnlich der Installationsanleitung im [Padlet](https://pad.gwdg.de/Pc0xEV7zSh2wBKLFvjgAow?both#Installation-und-Konfiguration-von-Koha) gefolgt. 

![Screenshot from 2020-06-28 21-04-34](Sitzung02.assets/Screenshot from 2020-06-28 21-04-34.png)

Login-Screen der Koha-Installation in einer “nativen” Ubuntu-VM.



