# ****PHOTOVERIFY_IOS****

## Project Mandates
- **Doel:** iOS variant van het PhotoVerify ecosysteem.
- **Scope:** Native iOS forensics via Swift + Capacitor bridge.
- **Master Copy:** Georkestreerd door Meta_PhotoVerify.
- **Tech Stack:** React 19, TypeScript 5, Swift, Capacitor.
- **GitHub:** `https://github.com/cpaglebbeek/PhotoVerify_IOS.git` (branch: `main`)
- **Lokaal pad:** `/Users/christian/Documents/Gemini_Projects/PhotoVerify_IOS`

## Context-Aware Orchestration
- Platform-specifieke wijzigingen hier; core-logica ALTIJD in `Meta_PhotoVerify`.
- Na elke wijziging: automatisch `git commit` + `git push`.
- Elke reactie begint met: `****PHOTOVERIFY_IOS****`

## Feature & Bugfix Protocol (Color-Coded)
**Nieuwe Feature:**
- **Groen:** Minor → versie +0.0.1
- **Oranje:** Design impact → versie +0.1.0
- **Rood:** Architectural → versie +1.0.0

**Bugfix:**
- **Groen:** Snel herstel | **Geel:** Logisch niveau | **Rood:** Conceptueel + Security Audit | **Loop:** Nieuwe invalshoek

**Root Cause Analysis (verplicht):** Functioneel + Technisch + Architectonisch niveau.

## Build Mandate
- WhatIf analyse vóór elke build, daarna akkoord vragen.
- Change detection via `git status` vóór build.
- Nooit impliciet APK genereren vanuit iOS context.
- APK Delivery (indien Android build expliciet gevraagd): kopieer naar `/Users/christian/Downloads`.

## Versioning — Thema: Groundhog Day (facts)
- **GROEN:** +0.0.1 | **ORANJE:** +0.1.0 | **ROOD:** +1.0.0
- Unieke codenaam per build (Groundhog Day feit).
- Update `version.json`, `package.json`, Xcode build config vóór build/sync.

## Dashboard Update Mandate
Na elke build of versie-verhoging → update `dashboard_info.html` in Meta_PhotoVerify.
