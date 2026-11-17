<div align="center" id="top">
<img src="NxMotion Banner.jpg" alt="Nexus Motion Banner" width="100%" />

# NEXUS MOTION

### Official Release & Auto-Updater Repository

**Desktop-Class 3D Animation, Mobile RayTracing/PathTracing, Native SFM (.MDL) Support & Sandboxed Lua SDK.**

<br/>

[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20Android-000000?style=flat-square&logo=materialdesignicons&logoColor=white)](https://thedr1xx.itch.io/nexus-motion)
[![Engine](https://img.shields.io/badge/Engine-Godot%204.x-000000?style=flat-square&logo=godotengine&logoColor=white)](https://godotengine.org/)
[![Typography](https://img.shields.io/badge/Typography-Space%20Grotesk%20%26%20Inter-0A0A0D?style=flat-square&logo=googlefonts&logoColor=white)](https://fonts.google.com/)
[![Icons](https://img.shields.io/badge/Icons-Google%20Material%20Symbols-0A0A0D?style=flat-square&logo=materialdesign&logoColor=white)](https://fonts.google.com/icons)
[![License](https://img.shields.io/badge/License-Proprietary%20(All%20Rights%20Reserved)-18181B?style=flat-square)](./LICENSE)
[![Official Page](https://img.shields.io/badge/Download-Itch.io%20Official-FFFFFF?style=flat-square&logo=itchdotio&logoColor=black)](https://thedr1xx.itch.io/nexus-motion)

<br/>

[![English](https://img.shields.io/badge/Language-English-FFFFFF?style=for-the-badge&logo=googletranslate&logoColor=black)](#english)
&nbsp;&nbsp;
[![Español](https://img.shields.io/badge/Idioma-Cambiar%20a%20Español-0A0A0D?style=for-the-badge&logo=googletranslate&logoColor=white)](#español)

</div>

---

<div id="english"></div>

## ![Icon](https://img.shields.io/badge/-OVERVIEW-000000?style=flat-square&logo=materialdesignicons&logoColor=white) &nbsp; [EN] Overview

> **Language:** **English** &nbsp;|&nbsp; [Switch to Español](#español)

This repository serves as the **official distribution hub and automated update backend (OTA / Auto-Updater)** for **Nexus Motion**, developed by **Nexus Labs, Inc.**

> **Notice:** This repository hosts **compiled release binaries, update manifests (`version.json` / `latest.json`), cryptographic checksums, and distribution packages only**. The proprietary source code of Nexus Motion is closed-source and is not hosted in this repository.

**Nexus Motion** is a cross-platform 3D animation studio built to bring desktop-grade rigging, real-time rendering, world-building, and Source Filmmaker (SFM) workflows to both **PC (Windows / Linux)** and **Mobile (Android)** devices.

---

### ![Icon](https://img.shields.io/badge/-CORE%20CAPABILITIES-000000?style=flat-square&logo=materialdesign&logoColor=white) &nbsp; Core Capabilities

#### 1. Rendering & Visual Pipeline
- **Mobile & Desktop RayTracing / PathTracing:** Real-time global illumination, reflections, soft shadows, and multi-sample baking (`RayTraceBaker` & `RenderSuite`) optimized for both mobile GPUs and desktop hardware.
- **11 Viewport Visual Styles:** Instant switching between *Studio Standard*, *SEUS Ray-Traced GI*, *Complementary Reimagined*, *BSL Cinematic Bloom*, *Spider-Verse Comic*, *Anime Cel-Shading*, *CRT 90s*, *Vaporwave*, *Retro Voxel*, *35mm Film Grain*, and *Noir*.
- **Studio Pro Render Suite:** Multi-column render pipeline supporting `720p` up to `4K` (`2160p`), `24 / 30 / 60 FPS`, MP4/WebM/PNG sequence exports, physical Bokeh Depth of Field (DoF), Chromatic Aberration, 35mm Grain, LUT Color Grading (*IMAX, Cyberpunk, VHS 90s, Noir, Matrix, Golden Hour*), and transparent Alpha / Chroma Key passes.

#### 2. Rigging, Animation & Physics
- **Blender-Style Octahedral Bones (True X-Ray):** Global-space octahedral skeleton visualization with accurate joint picking across arbitrary `.fbx`, `.glb`, and `.mdl` import scales, plus automatic support for node-hierarchy rigid rigs.
- **Production Timeline (Studio Pro Mode):** Keyframe interpolation curves (*Linear, Cubic/Bezier, Ease-In/Out, Bounce, Elastic, Back, Stepped 12 FPS*), 3D Onion Skinning, `Time Scale` slow-motion tracks, multi-camera `Camera Switcher`, and visual Audio Waveforms.
- **Keyframe-Driven Bone Physics:** Non-destructive chain physics (hair, cloth, tails) and elastic jiggle controlled directly via timeline keyframes, plus rigid-body props, limb dismemberment, and 3D weapon/limb motion trails.

#### 3. Native Source Engine (.MDL / .VTF) & Steam Workshop Pipeline
- **Direct Source Asset Importing:** Native runtime parsing and assembly of Source Filmmaker / Source Engine models (`.mdl`), maps (`.vmf`), materials (`.vmt`), and textures (`.vtf`) without external conversion steps.
- **Hierarchy-Preserving Outliner:** Retains authentic internal folders, sub-meshes, and original bone names from imported archives (`.zip`, `.fbx`, `.glb`, `.mdl`).
- **Steam Workshop Integration:** Direct item lookup and importing workflow for SFM assets across supported platforms.

#### 4. World Builder, Weather & Skies
- **Real-Time Terrain & Localized Water:** Sculptable terrain heightmaps with 3D brush cursors, localized water cavity painting (zero global Z-fighting), and accumulative `MultiMesh` foliage painting.
- **Scalable 3-Tier Cloud Engine:** Switch dynamically between *Lightweight 2D Skybox*, *Balanced 3D Volumetrics*, and *Ultra Realistic Volumetric Clouds* (`SunshineClouds2`).
- **Infinite Camera-Tracked Weather & Skies:** Dynamic 24-hour Day/Night cycle with procedural Sun, Moon, Starfield, pure `#000000` AMOLED mode, unlit Chroma Key mode, and infinite camera-following weather (*3D Rain with wind tilt, Snow, Volcanic Ash & Embers, and Electrical Thunderstorms with procedural lightning*).

#### 5. Sandboxed Lua 5.4 Plugin SDK & Cloud Asset Store
- **Zero-Trust Lua Sandbox:** Community creators can build `.nxplugin` extensions that add custom Inspector tabs, toolbar buttons, bone modifiers, and timeline generators without access to `res://`, network sockets, OS processes, or user files outside their isolated sandbox.
- **Cloud Asset Store:** Browse, filter by OS compatibility (*Windows, Mobile, Cross-Platform*), and install community plugins directly inside the application.

---

### ![Icon](https://img.shields.io/badge/-PLATFORMS%20%26%20DOWNLOADS-000000?style=flat-square&logo=googleplay&logoColor=white) &nbsp; Supported Platforms & Downloads

Official builds are distributed via **Itch.io** and mirrored through **GitHub Releases** for the automated in-app updater:

| Platform | Architecture | Graphics Backend | Minimum Requirements | Official Distribution |
| :--- | :--- | :--- | :--- | :--- |
| **Windows** | `x86_64` (64-bit) | Vulkan 1.2+ / DirectX 12 / OpenGL 3.3 | Windows 10/11, 4 GB RAM, GPU with Vulkan or OpenGL 3.3 support | [Download on Itch.io](https://thedr1xx.itch.io/nexus-motion) / [Releases](../../releases) |
| **Android** | `arm64-v8a` | Vulkan 1.1+ / OpenGL ES 3.0 | Android 9.0+, 4 GB RAM (6 GB+ recommended for PathTracing) | [Download on Itch.io](https://thedr1xx.itch.io/nexus-motion) / [Releases](../../releases) |
| **Linux** | `x86_64` (64-bit) | Vulkan 1.2+ / OpenGL 3.3 | Ubuntu 22.04+ or equivalent, 4 GB RAM | [Releases](../../releases) |

---

### ![Icon](https://img.shields.io/badge/-AUTO--UPDATER%20ARCHITECTURE-000000?style=flat-square&logo=googledrive&logoColor=white) &nbsp; Auto-Updater Architecture

When **Nexus Motion** launches, its built-in update client queries this repository to check for newer builds without interrupting user sessions:

1. **Manifest Check:** The client fetches the latest release metadata (`version.json` / GitHub Releases API) over HTTPS.
2. **Semantic Version Comparison:** Compares the local client build tag (`vX.Y.Z`) against the latest published release tag.
3. **Platform & Architecture Matching:** Selects the appropriate binary artifact (`.exe` / `.zip` for Windows, `.apk` for Android, `.x86_64` for Linux).
4. **Integrity Verification:** Validates file size and SHA-256 checksums before prompting the user to apply the update.

#### Repository Structure

```text
nexus-motion-releases/
├── LICENSE                 # Proprietary Binary Distribution & EULA License
├── NxMotion Banner.jpg     # Official repository banner
├── README.md               # Bilingual repository overview, architecture, and platform info
├── version.json            # Latest release manifest consumed by the in-app updater
└── changelogs/             # Release notes and version history
```

---

### ![Icon](https://img.shields.io/badge/-DESIGN%20SYSTEM%20%26%20TYPOGRAPHY-000000?style=flat-square&logo=googlefonts&logoColor=white) &nbsp; Design System, Typography & Iconography

**Nexus Motion** strictly adheres to the **Nexus Network AMOLED** design language:
- **Google Fonts Typography:**
  - **Display & Headings:** [`Space Grotesk`](https://fonts.google.com/specimen/Space+Grotesk) (SemiBold / Bold)
  - **UI & Body Copy:** [`Inter`](https://fonts.google.com/specimen/Inter) (Regular / Medium)
  - **Timeline & Numeric Data:** [`JetBrains Mono`](https://fonts.google.com/specimen/JetBrains+Mono) (Monospace)
- **Iconography:** 100% monochromatic **[Google Material Symbols](https://fonts.google.com/icons)** (`Outlined` / `Rounded` 20px–24px) — zero Unicode emojis across the entire application.
- **Surface Tokens:** Pure AMOLED `#000000` background, `#0A0A0D` elevated containers, `1px solid #1C1C21` hairline borders, and high-contrast `#FFFFFF` pill action buttons.

---

### ![Icon](https://img.shields.io/badge/-SECURITY%20%26%20INTEGRITY-000000?style=flat-square&logo=googlescholar&logoColor=white) &nbsp; Security & Integrity

- **Binary Encryption:** All official Windows, Linux, and Android builds are compiled with **GDScript bytecode encryption** enabled to protect intellectual property and prevent tampering.
- **Immutable Releases:** Published release tags and binary artifacts are locked against post-release modification to guarantee checksum consistency.
- **Sandboxed Extensions:** Third-party `.nxplugin` packages run strictly inside an isolated Lua 5.4 environment with explicit user permission prompts (`ui.inspector_tab`, `ui.toolbar_button`, `scene.edit`, `rig.bones`, `timeline.keyframes`).

---

### ![Icon](https://img.shields.io/badge/-SPECIAL%20THANKS-000000?style=flat-square&logo=materialdesign&logoColor=white) &nbsp; Special Thanks

A huge thank you to everyone who supported, tested, and helped push **Nexus Motion** forward:

| Contributor / Community | Recognition |
| :--- | :--- |
| **Gial Kraler** | Early support, testing, and feedback |
| **! $ax,,** | Hardware benchmarking, 4K RayTracing/PathTracing testing & feedback |
| **🔺• \| Red server \| •🔻** | Community support and server collaboration |
| **Every Nexus Motion User** | To everyone downloading, animating, creating plugins, and sharing renders with the program |

---

### ![Icon](https://img.shields.io/badge/-LEGAL%20%26%20LICENSING-000000?style=flat-square&logo=materialdesignicons&logoColor=white) &nbsp; Legal & Licensing

Copyright © 2026 **Nexus Labs, Inc. / TheDrixx**. All Rights Reserved.

All binaries, installers, update manifests, visual assets, and trademarks (`Nexus Motion`, `Nexus Labs`, `Nexus Network`) hosted in or referenced by this repository are governed by the **[Proprietary Software Distribution and Update License](./LICENSE)**.

- **Permitted:** Downloading and executing official packages for personal or internal use with an official installation of Nexus Motion.
- **Strictly Prohibited:** Redistributing, mirroring, re-uploading binaries to third-party sites, decompiling, reverse-engineering, decrypting `.pck`/`.apk`/`.exe` archives, or scraping manifests outside the official update workflow.

---

### ![Icon](https://img.shields.io/badge/-OFFICIAL%20LINKS-000000?style=flat-square&logo=googlechrome&logoColor=white) &nbsp; Official Links & Community

- **Official Storefront & DevLogs:** [https://thedr1xx.itch.io/nexus-motion](https://thedr1xx.itch.io/nexus-motion)
- **Releases & Update Packages:** [GitHub Releases](../../releases)
- **Developer:** Nexus Labs, Inc. (`TheDrixx`)

<div align="right">
  <a href="#top"><strong>[ Back to top ]</strong></a>
</div>

---
---

<div id="español"></div>

## ![Icon](https://img.shields.io/badge/-DESCRIPCIÓN%20GENERAL-000000?style=flat-square&logo=materialdesignicons&logoColor=white) &nbsp; [ES] Descripción General

> **Idioma:** [Switch to English](#english) &nbsp;|&nbsp; **Español**

Este repositorio funciona como el **centro oficial de distribución y servidor de actualizaciones automáticas (OTA / Auto-Updater)** para **Nexus Motion**, desarrollado por **Nexus Labs, Inc.**

> **Aviso:** Este repositorio aloja **únicamente binarios compilados oficiales, manifiestos de actualización (`version.json` / `latest.json`), sumas de verificación criptográficas y paquetes de distribución**. El código fuente propietario de Nexus Motion es cerrado y no se encuentra alojado en este repositorio.

**Nexus Motion** es un estudio de animación 3D multiplataforma diseñado para llevar herramientas de rigging de nivel de escritorio, renderizado en tiempo real, creación de mundos y flujos de trabajo de Source Filmmaker (SFM) tanto a **PC (Windows / Linux)** como a **dispositivos móviles (Android)**.

---

### ![Icon](https://img.shields.io/badge/-CAPACIDADES%20PRINCIPALES-000000?style=flat-square&logo=materialdesign&logoColor=white) &nbsp; Capacidades Principales

#### 1. Motor de Renderizado y Pipeline Visual
- **RayTracing / PathTracing en Móvil y PC:** Iluminación global en tiempo real, reflejos, sombras suaves y baking multimuestra (`RayTraceBaker` y `RenderSuite`) optimizados tanto para GPUs móviles como para hardware de escritorio.
- **11 Estilos Visuales en Viewport:** Cambio instantáneo entre *Studio Standard*, *SEUS Ray-Traced GI*, *Complementary Reimagined*, *BSL Cinematic Bloom*, *Spider-Verse Comic*, *Anime Cel-Shading*, *CRT 90s*, *Vaporwave*, *Retro Voxel*, *35mm Film Grain* y *Noir*.
- **Studio Pro Render Suite:** Pipeline de renderizado multicolumna compatible con resoluciones desde `720p` hasta `4K` (`2160p`), `24 / 30 / 60 FPS`, exportación en MP4/WebM/secuencias PNG, desenfoque de lente físico Bokeh (DoF), Aberración Cromática, Grano de cine 35mm, gradación de color LUT (*IMAX, Cyberpunk, VHS 90s, Noir, Matrix, Golden Hour*) y pases con fondo transparente Alpha / Chroma Key.

#### 2. Rigging, Animación y Físicas
- **Huesos Octaédricos Estilo Blender (X-Ray Real):** Visualización de esqueletos octaédricos en espacio global con selección precisa por articulación sin importar la escala de importación de archivos `.fbx`, `.glb` o `.mdl`, además de soporte automático para rigs articulados por jerarquía de piezas rígidas.
- **Línea de Tiempo de Producción (Modo Studio Pro):** Curvas de interpolación por keyframe (*Lineal, Cúbica/Bezier, Ease-In/Out, Rebote, Elástica, Back, Stepped 12 FPS*), Onion Skinning 3D, pista de cámara lenta `Time Scale`, selector multicámara `Camera Switcher` y visualización de ondas de audio (`Audio Waveform`).
- **Físicas de Huesos Controladas por Keyframes:** Físicas no destructivas en cadenas de huesos (cabello, telas, colas) y rebote elástico controlables directamente desde el Timeline, además de props rígidos, desmembramiento de extremidades y estelas de movimiento 3D para armas y golpes.

#### 3. Soporte Nativo Source Engine (.MDL / .VTF) y Steam Workshop
- **Importación Directa de Assets Source:** Lectura y ensamblaje nativo en tiempo real de modelos de Source Filmmaker / Source Engine (`.mdl`), mapas (`.vmf`), materiales (`.vmt`) y texturas (`.vtf`) sin necesidad de herramientas externas de conversión.
- **Outliner con Jerarquías Reales:** Conserva las carpetas internas originales, sub-mallas y nombres reales de huesos de archivos comprimidos (`.zip`, `.fbx`, `.glb`, `.mdl`).
- **Integración con Steam Workshop:** Búsqueda e importación directa de contenido de SFM en las plataformas compatibles.

#### 4. World Builder, Clima y Cielos Dinámicos
- **Terreno Esculpible y Agua Localizada:** Mapas de altura editables en tiempo real con cursor de pincel 3D, pintura de agua localizada en cavidades (cero *Z-fighting* global) y pintura acumulativa de vegetación mediante `MultiMesh`.
- **Motor de Nubes Escalable en 3 Niveles:** Alterna dinámicamente entre *Skybox 2D Ligero*, *Nubes Volumétricas 3D Equilibradas* y *Nubes Volumétricas Ultra Realistas* (`SunshineClouds2`).
- **Clima Infinito que Sigue a la Cámara y Cielos Procedurales:** Ciclo dinámico Día/Noche de 24 horas con Sol, Luna, cielo estrellado procedural, modo `#000000` AMOLED puro, modo Chroma Key sin glow y clima infinito vinculado a la cámara (*Lluvia 3D inclinada por el viento, Nieve, Ceniza Volcánica y Brasas, y Tormentas Eléctricas con relámpagos procedurales*).

#### 5. SDK de Plugins en Lua 5.4 (Sandbox) y Asset Store en la Nube
- **Sandbox Lua Zero-Trust:** Los creadores de la comunidad pueden desarrollar extensiones `.nxplugin` que añaden pestañas al Inspector, botones en la barra lateral, modificadores de huesos y generadores en el Timeline, sin acceso alguno a `res://`, conexiones de red, procesos del sistema operativo ni archivos fuera de su carpeta aislada.
- **Asset Store en la Nube:** Explora, filtra por compatibilidad de sistema operativo (*Windows, Móvil, Multiplataforma*) e instala plugins de la comunidad directamente desde la aplicación.

---

### ![Icon](https://img.shields.io/badge/-PLATAFORMAS%20Y%20DESCARGAS-000000?style=flat-square&logo=googleplay&logoColor=white) &nbsp; Plataformas Soportadas y Descargas

Las compilaciones oficiales se distribuyen a través de **Itch.io** y se reflejan en **GitHub Releases** para el sistema de actualización automática dentro de la app:

| Plataforma | Arquitectura | Backend Gráfico | Requisitos Mínimos | Distribución Oficial |
| :--- | :--- | :--- | :--- | :--- |
| **Windows** | `x86_64` (64 bits) | Vulkan 1.2+ / DirectX 12 / OpenGL 3.3 | Windows 10/11, 4 GB RAM, GPU compatible con Vulkan u OpenGL 3.3 | [Descargar en Itch.io](https://thedr1xx.itch.io/nexus-motion) / [Releases](../../releases) |
| **Android** | `arm64-v8a` | Vulkan 1.1+ / OpenGL ES 3.0 | Android 9.0+, 4 GB RAM (6 GB+ recomendados para PathTracing) | [Descargar en Itch.io](https://thedr1xx.itch.io/nexus-motion) / [Releases](../../releases) |
| **Linux** | `x86_64` (64 bits) | Vulkan 1.2+ / OpenGL 3.3 | Ubuntu 22.04+ o equivalente, 4 GB RAM | [Releases](../../releases) |

---

### ![Icon](https://img.shields.io/badge/-ARQUITECTURA%20DEL%20UPDATER-000000?style=flat-square&logo=googledrive&logoColor=white) &nbsp; Arquitectura del Auto-Updater

Al iniciar **Nexus Motion**, su cliente de actualizaciones integrado consulta este repositorio en segundo plano sin interrumpir el trabajo del usuario:

1. **Consulta de Manifiesto:** El cliente obtiene los metadatos de la última versión (`version.json` / API de GitHub Releases) mediante HTTPS.
2. **Comparación Semántica de Versión:** Compara la etiqueta local (`vX.Y.Z`) con la última versión oficial publicada.
3. **Selección por Plataforma y Arquitectura:** Elige automáticamente el paquete correspondiente (`.exe` / `.zip` para Windows, `.apk` para Android, `.x86_64` para Linux).
4. **Verificación de Integridad:** Valida el tamaño de archivo y las sumas SHA-256 antes de solicitar confirmación para aplicar la actualización.

#### Estructura del Repositorio

```text
nexus-motion-releases/
├── LICENSE                 # Licencia Propietaria de Distribución de Binarios y EULA
├── NxMotion Banner.jpg     # Banner oficial del repositorio
├── README.md               # Documentación bilingüe del repositorio, arquitectura y plataformas
├── version.json            # Manifiesto de última versión consumido por el auto-updater
└── changelogs/             # Notas de lanzamiento e historial de versiones
```

---

### ![Icon](https://img.shields.io/badge/-SISTEMA%20DE%20DISEÑO%20Y%20FUENTES-000000?style=flat-square&logo=googlefonts&logoColor=white) &nbsp; Sistema de Diseño, Tipografía Google Fonts e Iconografía

**Nexus Motion** sigue estrictamente el lenguaje visual **Nexus Network AMOLED**:
- **Tipografía Google Fonts:**
  - **Títulos y Encabezados:** [`Space Grotesk`](https://fonts.google.com/specimen/Space+Grotesk) (SemiBold / Bold)
  - **Interfaz y Textos:** [`Inter`](https://fonts.google.com/specimen/Inter) (Regular / Medium)
  - **Línea de Tiempo y Valores Numéricos:** [`JetBrains Mono`](https://fonts.google.com/specimen/JetBrains+Mono) (Monoespaciada)
- **Iconografía:** 100% **[Google Material Symbols](https://fonts.google.com/icons)** monocromáticos (`Outlined` / `Rounded` 20px–24px) — cero emojis Unicode en toda la interfaz.
- **Tokens de Superficie:** Fondo negro AMOLED puro `#000000`, tarjetas elevadas `#0A0A0D`, bordes finos `1px solid #1C1C21` y botones de acción principales tipo píldora en blanco `#FFFFFF`.

---

### ![Icon](https://img.shields.io/badge/-SEGURIDAD%20E%20INTEGRIDAD-000000?style=flat-square&logo=googlescholar&logoColor=white) &nbsp; Seguridad e Integridad

- **Encriptación de Binarios:** Todas las compilaciones oficiales de Windows, Linux y Android se exportan con **encriptación de bytecode de GDScript** activada para proteger la propiedad intelectual y evitar alteraciones.
- **Releases Inmutables:** Las etiquetas y archivos binarios publicados están bloqueados contra modificaciones posteriores para garantizar la consistencia de los checksums.
- **Extensiones Aisladas (Sandbox):** Los paquetes `.nxplugin` de terceros se ejecutan estrictamente dentro de un entorno Lua 5.4 aislado con confirmación explícita de permisos por parte del usuario (`ui.inspector_tab`, `ui.toolbar_button`, `scene.edit`, `rig.bones`, `timeline.keyframes`).

---

### ![Icon](https://img.shields.io/badge/-AGRADECIMIENTOS%20ESPECIALES-000000?style=flat-square&logo=materialdesign&logoColor=white) &nbsp; Agradecimientos Especiales

Un agradecimiento especial a quienes apoyaron, probaron y ayudaron a impulsar **Nexus Motion**:

| Colaborador / Comunidad | Reconocimiento |
| :--- | :--- |
| **Gial Kraler** | Apoyo temprano, pruebas y retroalimentación |
| **! $ax,,** | Pruebas de rendimiento en hardware, benchmarks 4K RayTracing/PathTracing y feedback |
| **🔺• \| Red server \| •🔻** | Apoyo comunitario y colaboración desde el servidor |
| **Todos los que usan el programa** | A cada creador que descarga, anima, desarrolla plugins y comparte sus renders con Nexus Motion |

---

### ![Icon](https://img.shields.io/badge/-ASPECTOS%20LEGALES%20Y%20LICENCIA-000000?style=flat-square&logo=materialdesignicons&logoColor=white) &nbsp; Aspectos Legales y Licencia

Copyright © 2026 **Nexus Labs, Inc. / TheDrixx**. Todos los derechos reservados.

Todos los binarios, instaladores, manifiestos de actualización, recursos visuales y marcas comerciales (`Nexus Motion`, `Nexus Labs`, `Nexus Network`) alojados o referenciados en este repositorio se rigen por la **[Licencia de Distribución y Actualización de Software Propietario](./LICENSE)**.

- **Permitido:** Descargar y ejecutar los paquetes oficiales para uso personal o interno junto con una instalación oficial de Nexus Motion.
- **Estrictamente Prohibido:** Redistribuir, crear copias espejo (*mirrors*), resubir binarios a sitios de terceros, descompilar, realizar ingeniería inversa, desencriptar archivos `.pck`/`.apk`/`.exe` o extraer manifiestos de forma automatizada fuera del flujo oficial de actualización.

---

### ![Icon](https://img.shields.io/badge/-ENLACES%20OFICIALES-000000?style=flat-square&logo=googlechrome&logoColor=white) &nbsp; Enlaces Oficiales y Comunidad

- **Página Oficial y DevLogs:** [https://thedr1xx.itch.io/nexus-motion](https://thedr1xx.itch.io/nexus-motion)
- **Releases y Paquetes de Actualización:** [GitHub Releases](../../releases)
- **Desarrollador:** Nexus Labs, Inc. (`TheDrixx`)

<div align="right">
  <a href="#top"><strong>[ Volver arriba ]</strong></a>
</div>
