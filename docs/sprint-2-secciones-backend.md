# Guía de contenido — Secciones Backend del Sprint 2

> **Propósito de este documento.** Antes de redactar las secciones del Sprint 2 que aún
> faltan, aquí se documenta **qué va en cada parte**, analizando cómo se llenaron las
> secciones equivalentes del **Sprint 1** (que sí están completas en el `README.md`).
> Este archivo es solo una **guía de referencia interna**: con esta información luego
> llenaremos las secciones reales del informe acorde a **X número de servicios** del
> backend (`kiniot/uflex-rest-api`).

---

## Contexto: diferencia entre Sprint 1 y Sprint 2

| Aspecto | Sprint 1 | Sprint 2 |
|---|---|---|
| Alcance principal | Front-end: Landing Page + Web App (PWA) | **Backend: monolito REST API** (Java + Spring Boot) + Edge + IoT/Embedded |
| Repositorios | `uflex-landing-page`, `uflex-clinic-web` | **`uflex-rest-api`** (y los repos de Edge/Embedded según corresponda) |
| Web Services | No aplicaban (se difirieron) | **Sí aplican** — son el centro del Sprint |
| Deployment | Vercel (front-end estático) | **Railway** (backend ya desplegado) |
| Documentación de servicios | No aplicaba | **Scalar / OpenAPI** (UI de documentación de la API) |

Por eso las cuatro secciones que faltan (`6.2.2.4`, `6.2.2.7`, `6.2.2.8`, `6.2.2.9`) en el
Sprint 2 se centran en el **backend**, a diferencia del Sprint 1 donde miraban al front-end.

**Estado actual del Sprint 2 en el `README.md`:**

- ✅ `6.2.2.1` Sprint Planning 2 — hecho
- ✅ `6.2.2.2` Aspect Leaders and Collaborators — hecho
- ✅ `6.2.2.3` Sprint Backlog 2 — hecho
- ⬜ **`6.2.2.4` Development Evidence for Sprint Review — FALTA**
- ✅ `6.2.2.5` Testing Suite Evidence — hecho
- ⬜ `6.2.2.6` Execution Evidence — (no solicitado en este pedido)
- ⬜ **`6.2.2.7` Services Documentation Evidence — FALTA**
- ⬜ **`6.2.2.8` Software Deployment Evidence — FALTA**
- ⬜ **`6.2.2.9` Team Collaboration Insights — FALTA**

---

## 6.2.2.4. Development Evidence for Sprint Review

### Qué es
Evidencia de los **commits** realizados durante el Sprint en los repositorios del alcance.
Demuestra el trabajo de desarrollo efectivamente entregado.

### Qué va aquí (basado en `6.2.1.4` del Sprint 1)
1. **Párrafo introductorio**: explica en qué se enfocó el equipo durante el Sprint y qué
   producto/módulos se implementaron. En el Sprint 1 se dijo "nos enfocamos en la Landing
   Page y la Web App". En el Sprint 2 corresponde decir que el foco fue el
   **monolito REST API** (`uflex-rest-api`) y sus bounded contexts.
2. **Por cada repositorio**:
   - Subtítulo en negrita con el nombre del repositorio.
   - `URL del repositorio: https://github.com/kiniot/...`
   - Un párrafo breve describiendo qué se implementó ahí.
   - **Tabla de commits** con estas columnas exactas:

     | Columna | Contenido |
     |---|---|
     | Repository | `kiniot/uflex-rest-api` |
     | Branch | rama del commit (ej. `feature/organization`, `feature/x → develop` para merges) |
     | Commit Id | hash corto (7 chars) |
     | Commit Message | título del commit (en inglés, conventional commits) |
     | Commit Message Body | descripción extendida o `—` si no tiene |
     | Committed on (Date) | fecha `DD/MM/2026` |

### Para el Sprint 2 (backend)
- Repositorio principal: **`kiniot/uflex-rest-api`**.
- Agrupar los commits por bounded context / feature: Organization, Device, Planning,
  Therapy, IAM, Subscription (alineado al Sprint Backlog `6.2.2.3`).
- Los merges hacia `develop` se documentan con notación `feature/x → develop`.

### Cómo obtener los datos
```bash
# Clonar/ubicarse en el repo del backend y listar commits con formato de tabla
git log --pretty=format:"%h | %s | %ad" --date=format:"%d/%m/2026" develop
# Para ver el cuerpo del commit:
git log --pretty=format:"%h%n%s%n%b%n---"
```
> ⚠️ Estos commits provienen de **`uflex-rest-api`**, NO de este repo del informe.

---

## 6.2.2.7. Services Documentation Evidence for Sprint Review

### Qué es
Documentación de los **Web Services (endpoints REST)** entregados, mostrada a través de la
UI de documentación de la API (**Scalar**, equivalente moderno de Swagger/OpenAPI).

### Qué va aquí
> En el Sprint 1 esta sección **no aplicaba** (texto que decía que se haría en el Sprint 2).
> En el Sprint 2 **sí se llena de verdad**. La estructura solicitada (mencionada en el
> propio texto de `6.2.1.7`) es:

1. **Párrafo introductorio**: indicar que la API está documentada con **Scalar/OpenAPI** y
   dónde está disponible (URL pública del Scalar desplegado en Railway, si aplica).
2. **Por cada servicio / endpoint** (aquí es donde entra el **"X número de servicios"**),
   documentar:
   - **Verbo HTTP** (GET, POST, PUT, DELETE…).
   - **Sintaxis de la llamada** (path del endpoint, ej. `POST /api/v1/sessions`).
   - **Parámetros** (path, query, body).
   - **Ejemplo de request** (JSON).
   - **Ejemplo de response** (JSON + código de estado).
   - **Captura de la UI de Scalar** mostrando ese endpoint.
3. **Capturas** de la interfaz de Scalar desplegada.
4. Opcionalmente, **commits asociados** a la documentación de servicios.

### Sugerencia de organización (acorde a X servicios)
Agrupar los endpoints por bounded context y dentro listar cada operación. Ejemplo de tabla
resumen antes del detalle:

| Bounded Context | Endpoint | Verbo | Descripción | User/Technical Story |
|---|---|---|---|---|
| Therapy | `/api/v1/sessions` | POST | Registrar sesión de rehabilitación | TS34 |
| Planning | `/api/v1/patients/{id}/metrics` | GET | Consultar métricas del paciente | TS35 |
| … | … | … | … | … |

> Cuando tengamos definido **cuántos y cuáles servicios** vamos a documentar, esta tabla se
> expande y por cada fila se agrega el bloque detallado con su captura de Scalar.

### Cómo obtener los datos
- Abrir el Scalar/OpenAPI del backend desplegado y tomar capturas por endpoint.
- El `openapi.json` / `openapi.yaml` del backend lista todos los endpoints, parámetros y
  schemas — es la fuente de verdad para llenar parámetros y ejemplos.

---

## 6.2.2.8. Software Deployment Evidence for Sprint Review

### Qué es
Evidencia del **despliegue** del software en el proveedor cloud. En el Sprint 1 fue
**Vercel** (front-end); en el Sprint 2 es **Railway** (backend ya desplegado).

### Qué va aquí (basado en `6.2.1.8` del Sprint 1)
1. **Párrafo introductorio**: indicar que se desplegó el backend en **Railway** y por qué.
2. **Por cada producto/servicio desplegado**:
   - Subtítulo en negrita (ej. **Despliegue — REST API**).
   - `URL pública: <https://...railway.app/>`
   - **Lista numerada de pasos realizados** durante el Sprint. En el Sprint 1 el patrón fue:
     1. Creación del proyecto en el proveedor.
     2. Importación / conexión del repositorio (rama de producción).
     3. Configuración del build (variables de entorno, base de datos, etc.).
     4. Verificación del dominio público y del estado **Ready / Active**.
   - **Captura del dashboard** del proveedor mostrando el deployment activo, dentro de un
     `<div style="text-align: center;">` con su `<img>`.
   - **Pie de figura** en cursiva: `*Figura 6.2.2.8.N. Railway — proyecto y despliegue de ...*`

### Para el Sprint 2 (Railway)
- Documentar el despliegue del **monolito REST API** en Railway.
- Si la base de datos (PostgreSQL/MySQL) y el Scalar también están en Railway, mencionar
  esos servicios del proyecto.
- Incluir la URL pública del backend y captura del panel de Railway con estado activo.

### Cómo obtener los datos
- Dashboard de Railway → proyecto del backend → tomar captura del deployment activo y copiar
  la URL pública generada.

---

## 6.2.2.9. Team Collaboration Insights during Sprint

### Qué es
Evidencia de la **colaboración del equipo**, usando los analíticos de **GitHub Insights**
del/los repositorio(s) del Sprint. En el Sprint 1 se hizo sobre los repos de front-end; en
el Sprint 2 corresponde hacerlo sobre el **backend** (`uflex-rest-api`).

### Qué va aquí (basado en `6.2.1.9` del Sprint 1)
1. **Párrafo introductorio**: explicar cómo se distribuyó el trabajo entre los integrantes
   y cómo se coordinó (dailies, revisión de PRs, etc.). Alinear con la matriz de leaders y
   collaborators de `6.2.2.2`.
2. **Por cada repositorio**, incluir capturas de **GitHub → Insights** con sus tres vistas
   estándar (cada una dentro de su `<div>` centrado + pie de figura en cursiva):
   - **Contributors** (`insights/contributors`).
   - **Commits over time** (`insights/commit-activity` o la pestaña de commits).
   - **Network graph** (`network`).
3. **Interpretación del equipo**: una breve lectura de lo que muestran los gráficos.

### Para el Sprint 2 (backend)
- Repositorio: **`kiniot/uflex-rest-api`** (y Edge/Embedded si el alcance lo incluye).
- Tomar las tres capturas de Insights por repositorio.

### Cómo obtener los datos
- GitHub → repo `uflex-rest-api` → pestaña **Insights**:
  - `https://github.com/kiniot/uflex-rest-api/graphs/contributors`
  - `https://github.com/kiniot/uflex-rest-api/graphs/commit-activity`
  - `https://github.com/kiniot/uflex-rest-api/network`

---

## Convenciones a respetar al llenar estas secciones

- **Numeración de figuras**: `Figura 6.2.2.<sección>.<n>` (ej. `Figura 6.2.2.8.1`).
- **Imágenes**: guardar en `assets/images/screenshots/sprint-2/` (las del backend ya
  existentes de testing están en `assets/testing/`). Mantener consistencia con la carpeta
  que se elija.
- **Patrón HTML de imagen** usado en el informe:
  ```html
  <div style="text-align: center;">
    <img src="assets/images/screenshots/sprint-2/<archivo>.png" alt="<alt>" style="max-width: 100%; height: auto;">
  </div>

  *Figura 6.2.2.X.N. <descripción>.*
  ```
- **Idioma**: el contenido del informe en **español**; los **mensajes de commit en inglés**.
- **Índice (TOC)**: al crear las secciones reales en el `README.md`, agregar también sus
  entradas en la tabla de contenidos (alrededor de las líneas 344–349, siguiendo el patrón
  de `6.2.1.x`).

---

## Resumen de fuentes de datos por sección

| Sección | Fuente principal | Formato de evidencia |
|---|---|---|
| 6.2.2.4 Development Evidence | `git log` de `uflex-rest-api` | Tabla de commits |
| 6.2.2.7 Services Documentation | Scalar/OpenAPI del backend | Tabla + detalle por endpoint + capturas |
| 6.2.2.8 Software Deployment | Dashboard de Railway | Pasos numerados + captura + URL |
| 6.2.2.9 Team Collaboration | GitHub Insights de `uflex-rest-api` | 3 capturas (contributors, commits, network) |
