# Biblioteca privada respaldada con LFS

Los artículos, libros, datasheets y tablas de apoyo de esta carpeta se indexan como punteros Git LFS. Los bytes se guardan en el folderstore privado de OneDrive y no en GitHub.

Después de un clon sin contenido LFS, ejecute `../scripts/configure-lfs-folderstore.ps1` y luego `../scripts/hydrate-lfs.ps1 -All`, o seleccione solamente una subcarpeta con `-Include`. Las notas conservan sus enlaces relativos originales.
