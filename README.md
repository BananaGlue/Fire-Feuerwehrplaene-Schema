# Georeferenzierte Feuerwehrpläne

Datenschema zur Validierung von georeferenzierten Feuerwehrplandaten nach den Vorgaben des Technischer Berichtes der vfdb – Referat 7 zur
DIN 14095:2024-01 Anhang B in der Version `vfdb TB 07-01:2026-01`: https://www.vfdb.de/media/doc/technischeberichte/TB_07-01_Technischer_Bericht_georeferenzierte_Feuerwehrplaene.pdf.

Es sind 8 Punktebenen, zwei Linienebenen und eine Flächenebene definiert, mit den folgenden Ebenennamen:

### Punktebenen:
- p_adresspunkt
- p_brandmeldezentrale
- p_zufahrt_zugang
- p_loeschwasserversorgung
- p_vertikaleerschliessung
- p_besonderegefahren
- p_vorbeugenderbaulicherbrandschutz
- p_sonstigesymbole

### Linienebenen:
- l_vorbeugenderbaulicherbrandschutz
- l_feuerwehrzufahrten

### Flächenebene:
- f_vorbeugenderbaulicherbrandschutz

Die Dateien sind wie im folgenden beschrieben zu benennen: `Feuerwehrplannummer_Ebenenname.geojson`. Alle Dateien sollen in einem Verzeichnis liegen, das nach der Feuerwehrplannummer benannt ist.
Lautet die zugewiesene Feuerwehrplannummer beispielsweise `170174` so wären die zu liefernden Dateien jeweils so zu bennen:

```
170174_p_adresspunkt.geojson
170174_p_brandmeldezentrale.geojson
170174_p_zufahrt_zugang.geojson
170174_p_loeschwasserversorgung.geojson
170174_p_vertikaleerschliessung.geojson
170174_p_besonderegefahren.geojson
170174_p_vorbeugenderbaulicherbrandschutz.geojson
170174_p_sonstigesymbole.geojson
170174_l_vorbeugenderbaulicherbrandschutz.geojson
170174_l_feuerwehrzufahrten.geojson
170174_f_vorbeugenderbaulicherbrandschutz.geojson
```

Die Daten haben je nach Ort des Gebäudes im amtlichen Lagebezugsystem ETRS89/ UTM Zone 32 (EPSG: 25832) bzw. Zone 33 (EPSG:
25833) zu erfolgen. Die Vorgabe des zu verwendenen Systems erfolgt durch die örtliche Feuerwehr.

Es ist utf-8 als Zeichensatz zu verwenden.

Die Datentypen orientieren sich an den Beispielen des technischen Berichtes: ja / nein ist als Integer `1 / 0` umgesetzt und das Datum als `TT.MM.JJJJ` String.



