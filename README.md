# Airlines API – Manual & Exploratory Testing Portfolio

## Project Overview

This repository presents a comprehensive manual and exploratory testing project for the [cf-automation-airline-api](https://github.com/terranigmark/cf-automation-airline-api) demo API.  
All test cases, findings, and bug reports were developed as part of the **Testing Automation Bootcamp by Código Facilito**.

## Context

The main goal of this project is to demonstrate deep QA skills, including test design, boundary value analysis, exploratory testing, and detailed bug reporting on a real-world API.  
All work was performed independently by me, **Josué Tenorio**, using the API originally created by [@terranigmark](https://github.com/terranigmark).

---

## About the API

- **API:** Airlines management demo API (FastAPI, Python)
- **Original repository:** [cf-automation-airline-api](https://github.com/terranigmark/cf-automation-airline-api)
- **Focus endpoint:** `/auth/signup` (User Registration)

---

## Tools Used

- **Postman** (manual testing, environments, data-driven testing)
- **Excel** and **Google Sheets** (test documentation, reporting)
- **GitHub Issues** (bug reporting, issue tracking)

---

## Testing Approach & Methodology

- **Manual testing:** All test cases were executed manually using Postman.
- **Test design techniques:**
  - Functional tests (positive and negative)
  - Boundary value analysis and equivalence partitioning
  - Exploratory and non-functional tests (e.g., large inputs, Unicode, security edge cases)
  - Security and input validation checks
- **Documentation:** Test results were recorded in both Excel and Google Sheets for transparency and reproducibility.

---

## File Organization

- `/postman/api-airlines.postman_collection.json`:  
  Complete **Postman collection** for this project.  
  You can import this file into Postman to easily replicate all requests (including signup, login, user, airport, flight, booking, and payment endpoints) and validate or expand the test scenarios described in this repo.
- [Google Sheets - Airlines API Test Cases (public)](https://docs.google.com/spreadsheets/d/1N8kPVLFH3IINNayiLmtJQllj9gmc0mOD/edit?usp=sharing&ouid=103821588095645487144&rtpof=true&sd=true): For easy review and sharing
- `airlines_api_test_cases.xlsx`: Backup of all manual test cases (included in this repo)
- `/github/issues`: All critical bugs were reported and tracked as GitHub Issues in this repository

---

## Key Bugs Found

The following critical bugs were discovered and reported during testing:

1. **[API-BUG-009]** Signup endpoint does not trim leading, trailing, or multiple spaces from `full_name` field  
   *Status: Open*

2. **[API-BUG-008]** Signup endpoint allows registration with `full_name` containing numbers  
   *Status: Open*

3. **[API-BUG-007]** Signup endpoint allows registration with `full_name` containing special characters  
   *Status: Open*

4. **[API-BUG-006]** Signup endpoint allows registration with empty `full_name` field  
   *Status: Open*

5. **[API-BUG-005]** Signup endpoint allows sign up with email addresses containing Unicode characters in the domain section  
   *Status: Open*

6. **[API-BUG-004]** Signup endpoint allows registration with email addresses containing Unicode characters in the local and domain sections  
   *Status: Open*

7. **[API-BUG-003]** Signup endpoint allows registration with email addresses having a top-level domain (TLD) of only 1 character  
   *Status: Open*

8. **[API-BUG-002]** Signup endpoint does not enforce a reasonable maximum length for `full_name` field  
   *Status: Open*

9. **[API-BUG-001]** Signup endpoint returns 500 error when password exceeds maximum length  
   *Status: Open*

> All issues can be reviewed directly in this repository's [Issues section](https://github.com/JosueTenorio99/cf-automation-airlines-api-auth-tests/issues).

---

## Skills Demonstrated

- Manual and exploratory API testing with professional documentation
- Boundary value and equivalence class analysis
- Security and input validation testing
- Defect reporting and root cause analysis
- Use of Postman environments and advanced requests
- Professional communication and bug tracking via GitHub Issues

---

## How to Review All Test Cases

- **Google Sheets (recommended for quick access):**  
  [Airlines API Test Cases – Google Sheets](https://docs.google.com/spreadsheets/d/1N8kPVLFH3IINNayiLmtJQllj9gmc0mOD/edit?usp=sharing&ouid=103821588095645487144&rtpof=true&sd=true)
- **Excel file (backup, included in this repo):**  
  `airlines_api_test_cases.xlsx`
- **Postman Collection (import into Postman to replay/validate scenarios):**  
  `/postman/api-airlines.postman_collection.json`

---

## Author

**Josué Tenorio**  
[LinkedIn](https://www.linkedin.com/in/josue-tenorio/)  
Email: tndjosue69@gmail.com

---

## Learning & Reflection

This project challenged me to design and execute test cases covering both functional and edge-case scenarios in a real-world API.  
Through manual testing and systematic documentation, I discovered several critical input validation issues, which are common pain points in backend development.  
I deepened my skills in exploratory testing, reporting actionable bugs, and communicating results clearly for developers and stakeholders.

---

---

---

# Airlines API – Pruebas Manuales y Exploratorias (Español)

## Descripción del Proyecto

Este repositorio presenta un proyecto completo de pruebas manuales y exploratorias sobre la [cf-automation-airline-api](https://github.com/terranigmark/cf-automation-airline-api).  
Todas las pruebas y reportes de bugs fueron realizados como parte del **Bootcamp de Testing Automatizado de Código Facilito**.

## Contexto

El objetivo principal de este proyecto es demostrar habilidades sólidas de QA, incluyendo el diseño de casos de prueba, análisis de valores límite, pruebas exploratorias y reporte profesional de bugs en una API real.  
Todo el trabajo fue realizado de forma independiente por mi, **Josué Tenorio**, utilizando la API original de [@terranigmark](https://github.com/terranigmark).

---

## Sobre la API

- **API:** API demo de gestión de aerolíneas (FastAPI, Python)
- **Repositorio original:** [cf-automation-airline-api](https://github.com/terranigmark/cf-automation-airline-api)
- **Endpoint principal probado:** `/auth/signup` (Registro de usuario)

---

## Herramientas Utilizadas

- **Postman** (pruebas manuales, environments, pruebas con datos)
- **Excel** y **Google Sheets** (documentación y reporte de pruebas)
- **GitHub Issues** (reporte y seguimiento de bugs)

---

## Enfoque y Metodología de Pruebas

- **Pruebas manuales:** Todos los casos fueron ejecutados manualmente en Postman.
- **Técnicas de diseño:**
  - Pruebas funcionales (positivas y negativas)
  - Análisis de valores límite y clases de equivalencia
  - Pruebas exploratorias y no funcionales (inputs extensos, Unicode, casos de seguridad)
  - Revisión de validaciones y manejo de errores
- **Documentación:** Todos los resultados fueron registrados en Excel y Google Sheets para transparencia y reproducibilidad.

---

## Organización de Archivos

- `/postman/api-airlines.postman_collection.json`:  
  **Colección completa de Postman** para este proyecto.  
  Puedes importar este archivo en Postman para replicar fácilmente todas las solicitudes (incluyendo endpoints de registro, login, usuarios, aeropuertos, vuelos, reservaciones y pagos) y validar o expandir los escenarios de prueba documentados aquí.
- [Google Sheets - Airlines API Test Cases (público)](https://docs.google.com/spreadsheets/d/1N8kPVLFH3IINNayiLmtJQllj9gmc0mOD/edit?usp=sharing&ouid=103821588095645487144&rtpof=true&sd=true): Acceso fácil y compartible
- `airlines_api_test_cases.xlsx`: Respaldo de todos los casos de prueba manual (incluido en el repo)
- `/github/issues`: Todos los bugs críticos fueron reportados y gestionados en los Issues de este repositorio

---

## Bugs Encontrados

Durante las pruebas se detectaron y reportaron los siguientes bugs críticos:

1. **[API-BUG-009]** El endpoint de registro no elimina espacios al inicio, al final, ni normaliza espacios múltiples en `full_name`  
   *Abierto*

2. **[API-BUG-008]** Permite registrar usuarios con números en `full_name`  
   *Abierto*

3. **[API-BUG-007]** Permite registrar usuarios con caracteres especiales en `full_name`  
   *Abierto*

4. **[API-BUG-006]** Permite registrar usuarios con `full_name` vacío  
   *Abierto*

5. **[API-BUG-005]** Permite registrar correos electrónicos con caracteres Unicode en el dominio  
   *Abierto*

6. **[API-BUG-004]** Permite registrar correos electrónicos con caracteres Unicode en la parte local y de dominio  
   *Abierto*

7. **[API-BUG-003]** Permite registrar correos electrónicos con TLD (dominio superior) de solo 1 carácter  
   *Abierto*

8. **[API-BUG-002]** No limita razonablemente la longitud máxima para el campo `full_name`  
   *Abierto*

9. **[API-BUG-001]** Retorna error 500 cuando el password excede la longitud máxima permitida  
   *Abierto*

> Todos los bugs pueden revisarse en la sección de [Issues](https://github.com/JosueTenorio99/cf-automation-airlines-api-auth-tests/issues) de este repositorio.

---

## Habilidades Demostradas

- Pruebas manuales y exploratorias de API con documentación profesional
- Análisis de valores límite y clases de equivalencia
- Pruebas de seguridad y validación de inputs
- Reporte de defectos y análisis de causa raíz
- Manejo avanzado de Postman y ambientes de prueba
- Comunicación profesional y seguimiento de bugs en GitHub

---

## Cómo Revisar Todos los Casos de Prueba

- **Google Sheets (recomendado):**  
  [Airlines API Test Cases – Google Sheets](https://docs.google.com/spreadsheets/d/1N8kPVLFH3IINNayiLmtJQllj9gmc0mOD/edit?usp=sharing&ouid=103821588095645487144&rtpof=true&sd=true)
- **Archivo Excel (incluido en el repo):**  
  `airlines_api_test_cases.xlsx`
- **Colección de Postman (importa en Postman para replicar/validar los escenarios):**  
  `/postman/api-airlines.postman_collection.json`

---

## Autor

**Josué Tenorio**  
[LinkedIn](https://www.linkedin.com/in/josue-tenorio/)  
Correo: tndjosue69@gmail.com

---

## Aprendizajes

Este proyecto me permitió diseñar y ejecutar pruebas cubriendo tanto escenarios funcionales como casos límite y exploratorios en una API real.  
Descubrí varios problemas críticos de validación de inputs, lo que es frecuente en desarrollos backend.  
Fortalecí mis habilidades en pruebas exploratorias, documentación y comunicación de resultados técnicos a equipos de desarrollo y stakeholders.

---
