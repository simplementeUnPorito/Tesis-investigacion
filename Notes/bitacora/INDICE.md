# Bitácora del Proyecto de Tesis
## Sistema de Ondas Superficiales con Geófonos ESP32-PSoC

> **Autor:** Elías David Álvarez  
> **Repo:** [simplementeUnPorito/Tesis](https://github.com/simplementeUnPorito/Tesis)  
> **Período:** Febrero – Septiembre 2026
> **Total de commits:** >230 | **Días documentados:** 67

---

Este índice agrupa todas las entradas de la bitácora por etapa del proyecto.

---

## Etapa 1 — Arranque y Marco Teórico (Feb–Mar 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-02-25 | [[2026-02-25]] | Commit inicial: repositorio creado |
| 2026-03-03 | [[2026-03-03]] | Vault Obsidian + resumen Capítulo 1 (Foti) |
| 2026-03-11 | [[2026-03-11]] | PDFs de Sebastiano Foti agregados al vault |
| 2026-03-13 | [[2026-03-13]] | Capítulo 2 completo + reorganización de Concepts |
| 2026-03-17 | [[2026-03-17]] | Submodulo MASW-Matlab, scripts teoría, startup.m |
| 2026-03-18 | [[2026-03-18]] | Scripts MATLAB teóricos + primer worklog |
| 2026-03-19 | [[2026-03-19]] | Capítulos 3, 4 y 5 resumidos + sesión nocturna masiva |
| 2026-03-20 | [[2026-03-20]] | Base de datos de papers + PDFs de investigación |
| 2026-03-23 | [[2026-03-23]] | Expansión masiva de la base de papers |

---

## Etapa 2 — Investigación IA Autónoma (Apr 10–15, 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-04-10 | [[2026-04-10]] | Revisión y limpieza de capítulos Obsidian |
| 2026-04-11 | [[2026-04-11]] | **GRAN SESIÓN** — Loop INVESTIGADOR: ~80 commits, 140 conceptos atómicos |
| 2026-04-12 | [[2026-04-12]] | Continuación INVESTIGADOR: Fases 5–6 completas, 4to ejemplo por capítulo |
| 2026-04-15 | [[2026-04-15]] | Cierre de la rama investigada por la IA |

---

## Etapa 3 — Hardware y Electrónica Analógica (Apr 17 – May 10, 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-04-17 | [[2026-04-17]] | MATLAB SM-24 empieza la locura |
| 2026-04-18 | [[2026-04-18]] | Más avances hardware |
| 2026-04-19 | [[2026-04-19]] | Loop auto-mejora Claude: PSoC FIR, ESP32 WiFi, 119 tests |
| 2026-04-22 | [[2026-04-22]] | LocuraCCp: datos reales del osciloscopio, compensador |
| 2026-04-27 | [[2026-04-27]] | Pruebas del circuito analógico |
| 2026-04-29 | [[2026-04-29]] | GeofonoSimplePruebaDeConcepto |
| 2026-04-30 | [[2026-04-30]] | Pre-locura cambios analógicos |
| 2026-05-05 | [[2026-05-05]] | Filtro notch + análisis espectral |
| 2026-05-10 | [[2026-05-10]] | Calibración manual, referencias desplazadas |

---

## Etapa 4 — Sistema Inalámbrico ESP-NOW (May–Jun 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-05-17 | [[2026-05-17]] | Primer sistema analógico funcionando |
| 2026-05-18 | [[2026-05-18]] | Lucha con el circuito analógico |
| 2026-05-20 | [[2026-05-20]] | PSoC + proyecto analógico LPF + datos masivos |
| 2026-05-24 | [[2026-05-24]] | ESP: nodo comunicación + refactor con Claude |
| 2026-05-25 | [[2026-05-25]] | HELLO beacon, START probe/ACK, debug pulses |
| 2026-05-26 | [[2026-05-26]] | PRESTART + scope multi-start → **¡Funciona!** |
| 2026-05-28 | [[2026-05-28]] | Debug y ajustes post-éxito |
| 2026-05-29 | [[2026-05-29]] | Más ajustes y estabilización |
| 2026-05-31 | [[2026-05-31]] | Refactor final: UART PSoC↔ESP, PR #2 mergeado |

---

## Etapa 5 — Producción y Debug Fino (Jun–Aug 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-06-03 | [[2026-06-03]] | Beacon fix 10Hz, VER store-and-forward, PSoC probe, UART 115200 → "Locura funciona super bien" |
| 2026-06-04 | [[2026-06-04]] | Workspace Martillo_ESP.cydsn — nodo PSoC+ESP para martillo de impacto |
| 2026-07-02 | [[2026-07-02]] | Nace `superMaquina`: captura migra de C a máquina de estados en hardware (Verilog) |
| 2026-07-07 | [[2026-07-07]] | Fs a 1020 Hz, dos rangos de ADC, circuit-breaker de tormenta de IRQ, arranque del pipeline MASW en Python |
| 2026-07-08 | [[2026-07-08]] | ADC de 2 a 4 rangos, RSSI de enlace en la web, doce fases de pulido en la revisión de campo + inversión MASW multimodal |
| 2026-07-09 | [[2026-07-09]] | Auditoría autocrítica (4 bugs corregidos), polaridad de geófono, enfase por carpeta, grupos de dispersión con combinación ponderada |
| 2026-07-11 | [[2026-07-11]] | Auditoría pre-campo: SD en PSoC validada en hardware real, fix de carrera en captura por USB, bug crítico F1 (aceptación 10 min, 0 muestras) encontrado y corregido en vivo |
| 2026-07-12 | [[2026-07-12]] | Cierre de la ampliación E12-E18 (todo PASS), bugs críticos F5 (dump colgado por socket zombie) y F9 (START rompía el nodo — race PRESTART/PSoC ARMED), regenerado FIR en PSoC |
| 2026-07-15 | [[2026-07-15]] | Paper Urucom: Secc. III/IV reescritas con datos reales (2 placas, barrido de ganancia), auto-revisión editorial simulada, flag `CAL_PI_FORCE_MIN_DEADBAND` para el experimento del estancamiento del PGA |
| 2026-07-16 | [[2026-07-16]] | Respuesta a la auto-revisión: 7 referencias nuevas, tabla de resultados con las 4 etapas, ecuaciones de banda muerta, corrección de honestidad sobre "Default" |
| 2026-07-20 | [[2026-07-20]] | Renombre GEO_ADDER→GEO_SUM en `psoc` (recalibración ganancia PI ×2.63, banda muerta configurable por etapa) + protocolo de barridos de la cadena analógica en `matlab` (zeta real del compensador ≈83.661 vs. objetivo 0.25) |
| 2026-07-21 | [[2026-07-21]] | Ruptura arquitectónica: monolito → superproyecto con 7 submódulos (root commit sin padres, LFS folder-backed); refactor AMux dedicados por etapa en `psoc` (`PGAshield`→`PGAout`, `LPF_2` activado) y modelo de circuito calibrado con `Ru=6.8kΩ` real en `matlab` |
| 2026-07-23 | [[2026-07-23]] | Paper URUCOM: compresión 6→5 páginas, panel de revisión simulado (Minor Revision, ≈65/100), sign test p≈10⁻³, reunión con el tutor; figura GEO→ADC side-by-side nueva en `matlab`; commit de `psoc` es solo regeneración de IDE |
| 2026-07-24 | [[2026-07-24]] | `src/` se reorganiza por propósito (no lenguaje): 6 submódulos (firmware/interfaces/calculos_modelados), 2 repos nuevos vía `subtree split`, `investigacion` migra a `docs/investigacion`; sketch `MasterFoo` valida hotspot del celular + plan de conectividad modo ENLACE del maestro |
| 2026-07-25 | [[2026-07-25]] | Arranca el PORT_PLAN del servidor `interfaces/python`: fix de gate (pipe de subprocess sin lector), migración a FastAPI + estáticos, tabs de navegación y toggle de tema, aclaración doc de las 4 funciones de filtrado, visor de señal con decimado min/max |
| 2026-07-26 | [[2026-07-26]] | Snapshot de referencia congelado de la app PyQt `field_review_app` en `docs/legacy/pyqt_field_review/`, con mapa de líneas de la ventana Capturas, antes de portarla entera a la web |
| 2026-07-29 | [[2026-07-29]] | Commit consolidado "Diseños 3d" (trabajo real del 26-27/07): cuarentena reversible en `deletion.py`, cola `AnalysisJobs`, gate `smoke_test.py` 58/58 checks; cierre de revisión URUCOM 2026 (IEEE membership, bibliografía BibTeX compartida) |
| 2026-08-01 | [[2026-08-01]] | "Se me acaba la bateria aaaa": pinout PSoC↔ESP32 migra a carrier intermedia (CY8CKIT-059+DevKitC) con verificación por script; arranca el martillo de leva en Simscape Multibody y Python (ambos detectan errores propios: interferencia axial leva-brazo y violación de energía); ajuste de fase en figura de auto-calibración URUCOM |

---

## Etapa 6 — Puesta en marcha de la placa (Sep 2026)

| Fecha | Archivo | Descripción |
|-------|---------|-------------|
| 2026-09-01 | [[2026-09-01]] | Primera placa digital APTA: I2C, UART, SYNC, captura E2E, SD y cinco botones; autotest usable, programación ECC 4×256 corregida y watchdog de ARMED |
| 2026-09-02 | [[2026-09-02]] | Auditoría documental del superproyecto: inventario de 11 repositorios, rutas/arquitectura corregidas, catálogo de datos ampliado y gate Markdown sin enlaces rotos |
| 2026-09-16 | [[2026-09-16]] | Síntesis 03–16/09: autocalibración de la cadena GEO, ganancia 96 sostenida (PGA ×4 · PGAout ×24), firmware PSoC unificado con PI permanente, telemetría I2C que perturba la cadena y modo estable |

---

## Tecnologías usadas en el proyecto

- **Obsidian** — Vault de conocimiento, notas de capítulos, conceptos atómicos
- **MATLAB/Simulink** — Modelos del geófono SM-24, análisis espectral, interfaz con hardware
- **PSoC (Cypress)** — Microcontrolador para adquisición analógica del geófono
- **ESP32/ESP8266** — Red inalámbrica ESP-NOW (maestro + esclavos) para transmisión de datos
- **Python** — Scripts de organización del vault Obsidian
- **Git** — Control de versiones (este repo)

---

*Generado automáticamente por Claude Code — Bitácora en construcción*
