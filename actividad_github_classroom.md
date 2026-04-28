# Plantilla de Propuesta de Tarea (Documentación Primero)

## 1) Título de la práctica
**Diseño de Mini Práctica Temática en Terminal**

> Puedes personalizar el título final de tu propuesta con algo más específico, por ejemplo:
> - Mini Toolkit en ARM64
> - Asistente de Estudio en Terminal
> - Reporteador de Información del Sistema
> - Organizador de Archivos
> - Juego de Aprendizaje en Línea de Comandos

---

## 2) Descripción general
En esta actividad **vas a diseñar** una propuesta de proyecto pequeño para terminal, con énfasis en **documentación, planeación y estructura del repositorio**.  
La meta es que primero justifiques bien la idea y su utilidad, y después (si el tiempo alcanza) implementes una versión mínima.

### Lenguaje principal (elige uno)
- ARM64 Assembly
- C
- Python
- Bash

> **Nota importante:** si eliges **ARM64 Assembly**, se recomienda que sea para programas **muy pequeños** (por ejemplo: operaciones básicas, manejo simple de texto, o utilerías mínimas).

### Restricciones de alcance
Para mantener el proyecto viable con herramientas gratuitas (Codex u otras IAs con límites), tu práctica debe ser:
- Pequeña y concreta.
- Ejecutable en entorno local.
- Sin frameworks pesados.
- Sin APIs pagadas.
- Sin bases de datos.
- Sin nube.
- Sin contenedores.
- Sin dependencias complejas.

---

## 3) Entregables del estudiante
Tu repositorio debe incluir, **como mínimo**:

- `README.md`
- `docs/propuesta.md`
- `docs/caso_de_uso.md`
- `docs/estructura_repositorio.md`
- `docs/plan_de_pruebas.md`

Opcional (si decides implementar algo):
- `src/`
- `scripts/`
- `tests/`

### Contenido esperado por archivo

#### `README.md`
Incluye:
1. Nombre del proyecto.
2. Problema que busca resolver.
3. Lenguaje elegido y justificación breve.
4. Alcance (qué sí hace y qué no hace).
5. Estructura del repositorio.
6. Instrucciones mínimas para ejecutar (si hay código).

#### `docs/propuesta.md`
Incluye:
1. Título de la práctica.
2. Objetivo general.
3. Objetivos específicos (3 a 5).
4. Público objetivo o contexto de uso.
5. Requerimientos funcionales mínimos.
6. Requerimientos no funcionales (simplicidad, portabilidad, legibilidad, etc.).
7. Justificación técnica del lenguaje elegido.
8. Alcance limitado de la primera versión (MVP).

#### `docs/caso_de_uso.md`
Incluye:
1. Escenario principal de uso narrado paso a paso.
2. Actor principal (quién usa la herramienta).
3. Entrada esperada.
4. Salida esperada.
5. Criterios de aceptación del caso de uso.

#### `docs/estructura_repositorio.md`
Incluye:
1. Árbol de carpetas propuesto.
2. Propósito de cada carpeta y archivo.
3. Convenciones de nombres.
4. Estrategia de crecimiento (cómo escalar sin romper orden).

#### `docs/plan_de_pruebas.md`
Incluye:
1. Qué se va a probar (comandos, funciones o flujos).
2. Casos de prueba mínimos (normal, borde y error).
3. Entradas y salidas esperadas por caso.
4. Evidencia esperada (capturas de terminal o logs simples).
5. Criterio de “práctica aceptable”.

---

## 4) Estructura recomendada del repositorio

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

> `<ext>` depende del lenguaje: `s` (ARM64), `c`, `py` o `sh`.

---

## Indicaciones de desarrollo (para el estudiante)

1. **Empieza por documentación**, no por código.
2. Define claramente el problema y limita el alcance.
3. Si implementas, que sea un prototipo pequeño y funcional.
4. Prioriza legibilidad y claridad sobre complejidad técnica.
5. Evita dependencias externas innecesarias.

---

## Rúbrica sugerida (100 puntos)

- **Claridad de la propuesta** (25 pts)
  - Objetivo claro, problema bien definido y enfoque realista.
- **Calidad de documentación** (30 pts)
  - Archivos completos, ordenados y coherentes entre sí.
- **Diseño de estructura del repositorio** (20 pts)
  - Organización limpia, nombres consistentes, fácil navegación.
- **Plan de pruebas** (15 pts)
  - Casos relevantes y criterios de aceptación claros.
- **Viabilidad técnica del alcance** (10 pts)
  - Proyecto pequeño, implementable y alineado al lenguaje elegido.

---

## Criterios de aceptación mínimos
Se considera **entrega válida** cuando:

- Existen todos los archivos obligatorios.
- La propuesta describe un proyecto pequeño y acotado.
- El caso de uso principal está bien explicado.
- La estructura del repositorio es coherente con la propuesta.
- El plan de pruebas incluye al menos 3 casos (normal, borde y error).

---

## Sugerencia de cronograma corto (opcional)

- **Día 1:** Definición del tema y lenguaje.
- **Día 2:** Redacción de `propuesta.md` y `caso_de_uso.md`.
- **Día 3:** Diseño de estructura y plan de pruebas.
- **Día 4 (opcional):** Implementación mínima y ajustes finales.

---

## Formato de entrega en GitHub Classroom
1. Crea tu repositorio desde la asignación.
2. Sube los archivos de documentación solicitados.
3. Verifica ortografía, consistencia y comandos.
4. Realiza commit final con mensaje sugerido:
   - `docs: propuesta inicial de práctica temática`
5. Entrega el enlace del repositorio según indicaciones del docente.
