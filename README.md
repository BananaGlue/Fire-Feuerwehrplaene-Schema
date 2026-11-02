# Georeferenzierte Feuerwehrpläne

Datenschema zur Validierung von georeferenzierten Feuerwehrplandaten nach den Vorgaben des Technischer Berichtes der vfdb – Referat 7 zur
DIN 14095:2024-01 Anhang B (https://www.vfdb.de/media/doc/technischeberichte/TB_07-01_Technischer_Bericht_georeferenzierte_Feuerwehrplaene.pdf).

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


Die Dateien sind wie im folgenden beschrieben zu benennen: `Feuerwehrplannummer_Ebenenname.geojson`
Lautet die zugewiesene Feuerwehrplannummer beispielsweise `170174` so wären die zu liefernden Dateien jeweils so zu bennen:

- 170174_p_adresspunkt.geojson
- 170174_p_brandmeldezentrale.geojson
- 170174_p_zufahrt_zugang.geojson
- 170174_p_loeschwasserversorgung.geojson
- 170174_p_vertikaleerschliessung.geojson
- 170174_p_besonderegefahren.geojson
- 170174_p_vorbeugenderbaulicherbrandschutz.geojson
- 170174_p_sonstigesymbole.geojson

- 170174_l_vorbeugenderbaulicherbrandschutz.geojson
- 170174_l_feuerwehrzufahrten.geojson

- 170174_f_vorbeugenderbaulicherbrandschutz.geojson

Die Daten haben je nach Ort des Gebäudes im amtlichen Lagebezugsystem ETRS89/ UTM Zone 32 (EPSG: 25832) bzw. Zone 33 (EPSG:
25833) zu erfolgen. Die Vorgabe des zu verwendenen Systems erfolgt durch die örtliche Feuerwehr.

Es ist utf-8 als Zeichensatz zu verwenden.



TODO:
add this to schema:
  "title": "p_vertikaleerschliessung",
  "crs": {
    "type": "name",
    "properties": {
      "name": "urn:ogc:def:crs:OGC:1.3:CRS84"
    }
  },


graphic

Brandschutzplaner erstellt / übersendet
pdf:
- Übersichtsplan
- Geschosspläne
- ...
geodaten:
- p_adresspunkt
- ...

VB / Planbüro / etc. empfängt / prüft / verwaltet

ELS / FIRE App / andere Systeme pflegen ein / stellen dar


