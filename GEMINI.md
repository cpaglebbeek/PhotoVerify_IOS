# PhotoVerify_IOS

## Project Mandates
- **Purpose:** iOS variant of the PhotoVerify ecosystem.
- **Scope:** Native iOS forensics using Swift and Capacitor.
- **Master Copy:** Orchestrated by Meta_PhotoVerify.
- **Tech Stack:** React 19, TypeScript 5, Swift, Capacitor.

## Context-Aware Orchestration Rule
- **Location Independence:** Het maakt niet uit in welke projectmap de gebruiker of AI zich bevindt. De AI MOET uit de context van het verzoek afleiden welk project (Meta, Android, iOS of Web) gewijzigd of gebouwd moet worden.
- **Routing:** Wijzigingen aan core-logica worden ALTIJD in `Meta_PhotoVerify` gedaan. Wijzigingen aan platform-specifieke bridges worden in het bijbehorende platform-project gedaan.
- **Syncing:** Na een wijziging moet de AI automatisch de git commit en push verzorgen voor de *gewijzigde* repository.
- **Explicit Context Formatting:** Elka reactie MOET beginnen met de projectnaam in HOOFDLETTERS tussen haakjes met sterretjes, exact zoals: <****PROJECTNAAM***>.
- **Explicit Context:**  Bij elk antwoord moet de AI expliciet vermelden op welk project de actie betrekking heeft.

## Context-Aware Orchestration Rule
- **Location Independence:** Het maakt niet uit in welke projectmap de gebruiker of AI zich bevindt. De AI MOET uit de context van het verzoek afleiden welk project (Meta, Android, iOS of Web) gewijzigd of gebouwd moet worden.
- **Routing:** Wijzigingen aan core-logica worden ALTIJD in `Meta_PhotoVerify` gedaan. Wijzigingen aan platform-specifieke bridges worden in het bijbehorende platform-project gedaan.
- **Syncing:** Na een wijziging moet de AI automatisch de git commit en push verzorgen voor de *gewijzigde* repository.
- **Explicit Context Formatting:** Elka reactie MOET beginnen met de projectnaam in HOOFDLETTERS tussen haakjes met sterretjes, exact zoals: <****PROJECTNAAM***>.
- **Explicit Context:**  Bij elk antwoord moet de AI expliciet vermelden op welk project de actie betrekking heeft.

## Feature & Bugfix Protocol (Color-Coded)
- **Nieuwe Feature:**
  - **Groen:** Minor (Code only, no design/arch impact).
  - **Oranje:** Design impact (Functional/Technical), but Logical Architecture remains stable.
  - **Rood:** Major impact (Redesign, Meta-implications, Conceptual/Logical/Physical shift).
- **Bugfix:**
  - **Groen:** Snel herstel (Fysiek niveau).
  - **Geel:** Out-of-physical-box (Logische architectuur van de oplossing).
  - **Rood:** Out-of-the-box (Conceptueel redesign + Security Audit).
  - **Loop:** Debug-loop (Probeer een compleet nieuwe invalshoek).
- **Root Cause Analysis (Mandatory):** Bij elke bugfix duid ik de oorzaak op drie niveaus: **Functioneel**, **Technisch**, en **Architectonisch abstractieniveau**.

## Build Delivery Mandate
- **APK Delivery:** Na elke succesvolle Android build MOET de resulterende APK gekopieerd worden naar `/Users/christian/Downloads`.

## Versioning Mandate
- **Mandatory Increment:** Elke functionele of technische wijziging MOET gepaard gaan met een verhoging van het versienummer in `version.json`, `package.json` en/of de platform-specifieke build-configuratie (Gradle/Xcode) vóórdat een build of sync plaatsvindt.

## Thematic Versioning & Naming Protocol
- **Versioning Logic (Semantic):**
  - **GROEN (Minor):** Increment .0.1 (bijv. 1.0.0 -> 1.0.1)
  - **ORANJE (Design):** Increment .1.0 (bijv. 1.0.1 -> 1.1.0)
  - **ROOD (Architectural):** Increment 1.0.0 (bijv. 1.1.0 -> 2.0.0)
- **Codename Theme:** Groundhog Day (Facts)
- **Uniqueness:** Elke build/oplevering MOET een unieke versie en een unieke thematische codenaam hebben.

## Dashboard Update Mandate
- **Ecosystem Visibility:** De `dashboard_info.html` in de Meta repository MOET bij elke build of versie-verhoging van elk project worden bijgewerkt met de meest actuele gegevens.
