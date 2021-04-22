B. Kießling
# Challenge 7: plotly und leaflet
## Zur Überprüfung dienen erneut die beiden Outputs (plot und map)

### plotly Verhältnis Arbeitlosigkeit und Migration -----------------------------

1. Lade den Datensatz stadtteil_profil_updated.rds in das Objekt stadtteile
2. Erstelle ein Scatter-Plot mit arbeitslosenanteil_in_percent_dez_2019 auf der y-Achse und anteil_der_bevolkerung_mit_migrations_hintergrund_in_percent auf der x-Achse
3. Löse das Problem beim Column arbeitslosenanteil_in_percent_dez_2019, sodass sich dieser richtig visualisieren lässt
> Tipp: Die Funktion as.numeric() wird dir dabei weiterhelfen
4. Runde die beiden zu visualierenden Columns auf eine Nachkommastelle
5. Beschrifte die x-Achse und y-Achse und erstelle einen Titel für den Plot
6. Nutze die Argumente text und hoverinfo und stelle die Hoverinfo wie im Beispieldiagramm dar
> Tipp: Für die Gestaltung der Hoverinformationen findest du alle Informationen hier: https://plotly.com/r/text-and-annotations/ im Abschnitt Custom Hover Text
7. Speichere den Plot mit htmlwidgets::saveWidget(as_widget(plotobject), "myfirstplot.html")
8. Interpretiere die Daten

### leaflet: Arbeitslosigkeit pro Stadtteil ----------------------------------

1. Lade den Datensatz stadtteile_wsg84.RDS in das Objekt stadtteile_gps
2. Benenne die Columns im Objekt stadtteile_gps von Stadtteil und Bezirk und stadtteil und bezirk um
3. Joine beide Datensätze in das Objekt stadtteile und nutze die Funktion %>% st_as_sf() am Ende der Pipe, um das Objekt als sf zu konvertieren
4. Erstelle ein leaflet Objekt und wähle ein Design über addProviderTiles(), 
5. Setze setView() auf (9.993682, 53.551086 = und wähle eine Zoom-Stufe
6. Ergänze die Code-Fragmente
7. Speichere die Map mit htmlwidgets::saveWidget(as_widget(mapobject), "myfirstmap.html")

# Wir werden die Map in der nächsten Einheit weiter gestalten!
