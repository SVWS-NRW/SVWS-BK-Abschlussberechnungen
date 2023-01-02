# SVWS-BK-Abschlussberechnungen
Ein Repo für die Algorithmen und die Dokumentation der Abschlussberechnungen am BK



## Installation der Projekte


**Download Eclipse**

https://www.eclipse.org/downloads/packages/

![SNAG_2022_12_11_12 24 55](https://user-images.githubusercontent.com/34127980/206900767-7b130135-cd75-446b-bb6d-d581e7a0c1c5.png)


**Entpacken des Zip Files und ggf Änderungen der Eclipse.ini zur Erhöung des Speichers:**

-Xms2048m
-Xmx32768m

**Eclipse Marketplace öffnen und nach Json suchen.**

Json viewer installieren.


**Neue Git-Perspektive öffnen und Projekt clonen:**

https://github.com/SVWS-NRW/SVWS-BK-Abschlussberechnungen

**Repository des SVWS-Server clonen und einrichten:**

https://github.com/SVWS-NRW/SVWS-Server

Im Verzeichnis .gradle eine gradle.properties anlegen.
Darin folgende Einträge ergänzen:

github_actor = githubnusername

github_token = ghp_eingueltigesgithubtoken

Dann in der Java Perspektive das Projekt als EXISTING GRADLEPROJEKT importieren.

Unter svws-server > svws-core > src/main/java befinden sich die Abschluss-Algorithmen:

![SNAG_2022_12_11_12 33 52](https://user-images.githubusercontent.com/34127980/206901182-8daba931-7864-4c87-b05e-28f2353862fb.png)



