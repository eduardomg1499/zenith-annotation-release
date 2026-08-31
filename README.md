# Zenith Annotation — descargas y actualizaciones

Este repositorio contiene únicamente las entregas publicadas de **Zenith
Annotation**, el editor científico local de anotaciones y resolución de placas
para astrofotografía de Zenith Astro Code. El código fuente no está aquí.

## Descargar

Ve a **[Releases](../../releases/latest)** y elige el archivo de tu sistema:

| Sistema | Archivo |
| --- | --- |
| macOS (Apple Silicon) | `Zenith-Annotation_<versión>_aarch64-apple-darwin.dmg` |
| Windows 10/11 x64 | `Zenith-Annotation_<versión>_x64-setup.exe` |

Junto a cada instalador se publica su `.sha256` para que puedas comprobar la
descarga.

En macOS:

```sh
shasum -a 256 -c Zenith-Annotation_<versión>_aarch64-apple-darwin.dmg.sha256
```

En Windows (PowerShell):

```powershell
Get-FileHash .\Zenith-Annotation_<versión>_x64-setup.exe -Algorithm SHA256
```

## Actualizaciones automáticas

La aplicación instalada consulta `latest.json` de este repositorio al arrancar y
te avisa cuando hay una versión nueva. Nada se descarga ni se instala sin que lo
aceptes, y la petición no envía datos de tu sesión ni identificadores de tu
equipo.

Los archivos `*.app.tar.gz`, `*.sig` y `latest.json` los usa ese actualizador:
no hace falta descargarlos a mano. Cada paquete va firmado y la aplicación
verifica la firma antes de aplicarlo.

## Soporte

- Web: <https://www.zenith-astro.com>
- Incidencias y sugerencias: [Issues](../../issues)

Zenith Annotation es software propietario de Zenith Astro Code. Las entregas de
este repositorio se distribuyen para su instalación y uso según la licencia que
acompaña a la aplicación.
