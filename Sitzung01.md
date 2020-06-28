# Sitzung 1

Datum: 13.03.2020

## Thema: Technische Grundlagen

#### Einrichtung der Arbeitsumgebung (Linux)

Nach ein paar ersten technischen Abklärungen haben wir uns daran  gemacht, eine virtuelle Linux-Maschine (Ubuntu 19.04 mit Xfce-Desktop) auf einer extra für die Klasse gemieteten Azure Workstation/Server zu  installieren. Wie es bei Microsoft oftmals vorkommt, haben sich viele von uns mit dem Microsoft-Account bzw. dem Login abgemüht, das für den  Azure-Zugang nötig ist. Da die Schul-Acounts partout nicht funktionierten, haben die meisten Studenten letzlich eine private Adresse verwendet.

Wir melden uns also mit unserem Microsoft-Account an und finden unsere assoziierten virtuellen Maschinen unter [ https://labs.azure.com]( https://labs.azure.com). Von dort aus können wir die Maschine entfernt hochfahren. Das Einloggen und Anzeigen des Systems erfolgt dann entweder per SSH im CLI (Command Line Interface) oder grafisch über das Remote Desktop-Protokoll. 

<img src="Sitzung01.assets/image-20200628150002020.png" alt="image-20200628150002020" style="zoom:50%;" />

Da ich wie bereits erwähnt, zumindest auf dem Desktop-Rechner, immer auf Linux arbeite, haben sich bei mir verschiedene Fragen zur Handhabung dieser VM gestellt bzw. ich habe verschiedene Zugriffsmöglichkeiten getestet. Zum einen gibt es die bekannteste Remote-Desktop-Lösung für Linux «[Remmina](https://remmina.org/)». Da ich auf einem UHD-Bildschirm arbeite war die Auflösung der VM leider immer ätzend klein (600x800 ca.), was ich auf die Schnelle leider auch nicht umstellen konnte. Deshalb versuchte ich mich noch mit einem CLI-Programm names *rdesktop*, das die VM einfach per Befehl aus dem Terminal startet. Ich habe dazu ein kleines Startskript geschrieben, das über eine .desktop-Datei dann ausgeführt wird. Der einzige Befehls-Parameter, den ich als Flag noch hinzugefügt hatte war “-g 100%”, was die Fenstergeometrie auf 100% skaliert und somit fast Fullscreen entspricht. 

Der Befehl zum Starten war dann letzlich folgender:

```bash
rdesktop-vrdp -g 100% ml-lab-1442cd48-fa24-4b5c-afdd-1ed4bb8bcb3d.northeurope.cloudapp.azure.com:54613
```

Im xfce-Desktop lässt sich unter Erscheinungsbild–>Einstellungen noch die Fensterskalierung auf “2x” setzen, was ein sehr annehmbares Resultat liefert – zumindest was die Auflösung betrifft. Die Performance ist nach vor sehr langsam und ruckelig, was natürlich nicht weiters überrascht. Deshalb hatte ich es mir zum Ziel gesetzt, soviele Programme und Installationen aus dem Unterricht direkt auf meinen Rechner nativ zu installieren, was nicht immer ganz glückte, wie wir noch sehen werden.

#### Grundlagen der Unix Shell

Unix Shell: I like! 

Soviel steht fest. Sie ist immens mächtig – ja, man kann sich das System sehr leicht zerschiessen und unter Umständen nicht mehr hochfahren. Aber diese Zeiten sind bei mir zum Glück eher vorbei. Nicht umsonst warnt einen Linux beim erstmaligen Benutzen von *sudo* über die damit verbundenen Gefahren. 

Im Unterricht machen wir also einen kleinen Exkurs in die Welt der CLI und manch einer hörte Begriffe wie *ls* oder *cd* zum ersten Mal. Ich kam zum Glück schon relativ früh mit der CLI und Linux in Kontakt, weil ich als Student in einer WG in Argentinien dringend WLAN brauchte und der Vermieter keinen Router in unserer Wohnung hatte – der Rest der Geschichte, naja, den lassen wir Geschichte sein ;-)

Herr Lohmeier hat uns auf die Seite [https://librarycarpentry.org/lc-shell/](https://librarycarpentry.org/lc-shell/) verwiesen, wo es tolle Übungen zur Shell gibt. Ich kannte sie selber nicht und hatte nicht so viel Zeit mich damit auseinaderzusetzen. Ist aber auf jeden Fall “ge-bookmarked”…

####  Versionskontrolle mit Git

Git, oh schönes Git…

Ja, Git und ich kennen uns schon etwas länger. So richtig innig wurde es aber erst dieses Jahr, als wir in einem anderen Fach (DGUI: Dynamic Graphical User Interfaces) offiziell damit arbeiten mussten für eine Projektarbeit. Und da es mir eigentlich sehr viel Spass macht, habe ich mich auch dazu entschieden, meine Blogs last Minute auf eine Github Page zu verschieben, da die Blogs ohnehin schon in Markdown geschrieben waren. Und das Zusammenspiel von GitHub, Markdown und erweitert durch Jekyll ist bekanntlich fliessend. 