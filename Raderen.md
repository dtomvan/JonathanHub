Dit was een test. Mocht je nou toch Obsidian hebben, dan kan je lekker losgaan op deze tabel jatoch.

```dataview
TABLE rows.file.link as Teksten
FROM #pensum-2024
SORT file.name asc
GROUP BY filter(file.etags, (x) => contains(["#2-symposion", "#6-gorgias", "#4-grotvergelijking", "#4-gyges"], x)) as Hoofdstuk
```
