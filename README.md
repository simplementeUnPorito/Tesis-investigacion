# Investigación y notas de Tesis

Vault de Obsidian con bitácora, notas conceptuales y trazabilidad académica de la tesis. Conserva el historial de las notas que antes estaban en `Obsidian Vault` dentro del monorepo.

Las copias de libros, artículos y datasheets se indexan en `sources/` mediante Git LFS. GitHub guarda solamente los punteros; los contenidos privados viven en `Github-LFS/repositories/Tesis-investigacion` y no se redistribuyen desde el repositorio público. Consulte `sources/README.md` para configurar e hidratar la biblioteca.

Puede abrir la raíz de este repositorio directamente como vault de Obsidian. En el superproyecto `Tesis` se monta en `investigacion`.

Configure el folderstore antes de hidratar fuentes:

```powershell
$env:GITHUB_LFS_ROOT = 'C:\Users\elias\OneDrive\Github-LFS'
.\scripts\configure-lfs-folderstore.ps1
.\scripts\hydrate-lfs.ps1 -Include 'sources/research/papers/pdf/**'
```
