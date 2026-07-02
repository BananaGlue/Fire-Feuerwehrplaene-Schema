# Georeferenzierte Feuerwehrpläne

Datenschema zur Validierung von georeferenzierten Feuerwehrplandaten nach den Vorgaben des Technischer Berichtes der vfdb – Referat 7 zur
DIN 14095:2024-01 Anhang B (https://www.vfdb.de/media/doc/technischeberichte/TB_07-01_Technischer_Bericht_georeferenzierte_Feuerwehrplaene.pdf).

Es sind 8 Punktebenen, zwei Linienebenen und eine Flächenebene definiert, mit den folgenden Ebenennamen:

- p_adresspunkt
- p_brandmeldezentrale
- p_zufahrt_zugang
- p_loeschwasserversorgung
- p_vertikaleerschliessung
- p_besonderegefahren
- p_vorbeugenderbaulicherbrandschutz
- p_sonstigesymbole

- l_vorbeugenderbaulicherbrandschutz
- l_feuerwehrzufahrt

- f_vorbeugenderbaulicherbrandschutz


Die Dateien sind wie im folgenden beschrieben zu benennen: `Feuerwehrplannummer_Ebenenname.geojson`
Lautet die zugewiesene Feuerwehrplannummer beispielsweise `170174` so wären die zu liefernden Dateien jeweils so zu bennen:

- 170174_p_adresspunkt.geojson
- 170174_p_brandmelderzentrale.geojson
- 170174_p_zufahrt_zugang.geojson
- 170174_p_loeschwasserversorgung.geojson
- 170174_p_vertikaleErschliessung.geojson
- 170174_p_besondereGefahren.geojson
- 170174_p_vorbeugenderBaulicherBrandschutz.geojson
- 170174_p_sonstigeSymbole.geojson

- 170174_l_vorbeugenderBaulicherBrandschutz.geojson
- 170174_l_feuerwehrzufahrt.geojson

- 170174_f_vorbeugenderBaulicherBrandschutz.geojson

Die Daten haben je nach Ort des Gebäudes im amtlichen Lagebezugsystem ETRS89/ UTM Zone 32 (EPSG: 25832) bzw. Zone 33 (EPSG:
25833) zu erfolgen. Die Vorgabe des zu verwendenen Systems erfolgt durch die örtliche Feuerwehr.







