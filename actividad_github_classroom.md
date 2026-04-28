# Plantilla de Propuesta de Tarea — Práctica Temática Documentada

## 1) Título de la práctica
**Diseño de Mini Práctica Temática en Terminal (Documentación Primero)**

> Ejemplos de tema (elige uno o propone otro equivalente):
> - *Mini Toolkit en ARM64*
> - *Asistente de Estudio en Terminal*
> - *Reporteador de Información del Sistema*
> - *Organizador de Archivos*
> - *Juego de Aprendizaje en Línea de Comandos*

---

## 2) Descripción general
En esta actividad **no se evalúa un sistema grande**, sino tu capacidad de **diseñar, justificar y documentar** una práctica técnica pequeña y viable para desarrollarse en pocas sesiones.

Vas a elaborar una **propuesta de proyecto** enfocada en:
- planteamiento del problema,
- caso de uso,
- estructura del repositorio,
- plan básico de pruebas,
- y alcance realista de implementación.

### Lenguaje principal (elige uno)
- **ARM64 Assembly**
- **C**
- **Python**
- **Bash**

> **Recomendación importante:** si eliges **ARM64 Assembly**, limita tu propuesta a un programa **muy pequeño** (por ejemplo: operaciones simples, lectura/escritura básica o utilidades mínimas de terminal).

### Enfoque de la actividad
Antes de escribir mucho código, debes demostrar que tu idea:
1. tiene un objetivo claro,
2. está acotada,
3. puede probarse,
4. y puede explicarse con buena documentación técnica.

---

## 3) Entregables del estudiante
Tu repositorio debe incluir, como mínimo, los siguientes archivos:

- `README.md`
- `docs/propuesta.md`
- `docs/caso_de_uso.md`
- `docs/estructura_repositorio.md`
- `docs/plan_de_pruebas.md`

Opcionales (si decides incluir implementación mínima):
- `src/`
- `scripts/`
- `tests/`

---

## 4) Estructura recomendada del repositorio
Usa esta estructura como base:

```text
nombre-del-proyecto/
├── README.md
├── docs/
│   ├── propuesta.md
│   ├── caso_de_uso.md
│   ├── estructura_repositorio.md
│   └── plan_de_pruebas.md
├── src/
│   └── main.<ext>
├── scripts/
│   └── run.sh
└── tests/
    └── test_plan.md
```

---

## 5) Instrucciones de contenido por archivo

### `README.md`
Incluye:
1. **Nombre del proyecto**.
2. **Resumen corto** (qué hace en 3–5 líneas).
3. **Lenguaje principal elegido** y por qué.
4. **Estado del proyecto** (propuesta / prototipo / parcial).
5. **Cómo ejecutar** (si ya hay código).
6. **Alcance y límites** (qué sí y qué no hará).

---

### `docs/propuesta.md`
Desarrolla estos apartados:
1. **Problema o necesidad** que atiende.
2. **Objetivo general**.
3. **Objetivos específicos** (3 a 5).
4. **Usuarios objetivo** (quién lo usaría).
5. **Alcance técnico** (funciones mínimas).
6. **Fuera de alcance** (lo que explícitamente no harás).
7. **Justificación del lenguaje** (ARM64/C/Python/Bash).
8. **Plan breve de implementación** por fases pequeñas.

---

### `docs/caso_de_uso.md`
Incluye:
1. **Nombre del caso de uso principal**.
2. **Actor principal**.
3. **Precondiciones**.
4. **Flujo principal** paso a paso.
5. **Flujos alternos o errores esperados**.
6. **Resultado esperado**.
7. **Ejemplo de entrada/salida** en terminal.

---

### `docs/estructura_repositorio.md`
Documenta:
1. **Árbol del repositorio** actualizado.
2. **Propósito de cada carpeta/archivo**.
3. **Convenciones de nombres** (archivos, scripts, funciones).
4. **Estrategia de crecimiento** (cómo escalar sin romper orden).

---

### `docs/plan_de_pruebas.md`
Debe contener:
1. **Objetivo de pruebas**.
2. **Tipos de pruebas mínimas** (funcional, entradas inválidas, borde).
3. **Casos de prueba en tabla**:
   - ID
   - Entrada
   - Acción
   - Resultado esperado
   - Resultado obtenido (cuando implementes)
4. **Criterios de aceptación** (qué debe cumplirse para darlo por válido).

---

## 6) Restricciones del proyecto
Para mantener la práctica viable en entornos con IA gratuita o limitada:

- Mantén el proyecto **pequeño y acotado**.
- Evita:
  - frameworks pesados,
  - APIs pagadas,
  - bases de datos,
  - servicios en la nube,
  - contenedores,
  - dependencias complejas.
- Prioriza herramientas locales de terminal y bibliotecas estándar del lenguaje.

---

## 7) Criterios de evaluación sugeridos (100%)

1. **Claridad de la propuesta y objetivos** — 25%
2. **Calidad del caso de uso** — 20%
3. **Estructura y organización del repositorio** — 20%
4. **Plan de pruebas realista y verificable** — 20%
5. **Coherencia técnica y alcance pequeño viable** — 15%

---

## 8) Recomendaciones por lenguaje

### Si eliges ARM64 Assembly
- Diseña una utilidad mínima (por ejemplo: calculadora básica de 2 operaciones, conversión simple o lectura/escritura elemental).
- No propongas parsers complejos ni menús extensos.

### Si eliges C
- Enfócate en entrada/salida en consola, archivos simples o utilidades de texto.
- Usa compilación directa con `gcc` o `clang` sin ecosistema extra.

### Si eliges Python
- Usa solo librería estándar.
- Prefiere scripts de línea de comandos (`argparse`, manejo de archivos, reportes simples).

### Si eliges Bash
- Automatiza tareas de archivos, validaciones o reportes de sistema.
- Cuida portabilidad y mensajes claros de error.

---

## 9) Entrega en GitHub Classroom
1. Acepta la asignación y crea tu repositorio.
2. Sube la estructura mínima con los archivos requeridos.
3. Completa primero la documentación en `docs/`.
4. (Opcional) agrega un prototipo mínimo en `src/` y script de ejecución.
5. Verifica que el `README.md` explique claramente cómo revisar tu propuesta.

---

## 10) Formato de entrega sugerido para el estudiante
Copia y pega esta checklist en tu `README.md` y márcala al finalizar:

- [ ] Definí un tema pequeño y viable.
- [ ] Elegí un lenguaje principal y lo justifiqué.
- [ ] Documenté objetivos y alcance en `docs/propuesta.md`.
- [ ] Escribí el caso de uso principal en `docs/caso_de_uso.md`.
- [ ] Expliqué la estructura del repo en `docs/estructura_repositorio.md`.
- [ ] Diseñé casos de prueba en `docs/plan_de_pruebas.md`.
- [ ] (Opcional) Implementé un prototipo mínimo.

---

## 11) Nota del docente
Esta actividad evalúa principalmente tu criterio de ingeniería para **acotar, estructurar y comunicar** una solución técnica. Una propuesta pequeña, bien pensada y bien documentada vale más que una implementación grande e incompleta.
