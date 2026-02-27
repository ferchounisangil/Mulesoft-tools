# 🛠️ Mulesoft Tools — Suratech

Colección de herramientas web para el equipo de desarrollo MuleSoft de **Suratech Insurtech**.
No requieren instalación ni dependencias — corren directo en el navegador.

---

## 📦 Herramientas disponibles

### 1. JSON Unescape
**Archivo:** `json-unescape.html`
**URL:** https://ferchounisangil.github.io/Mulesoft-tools/json-unescape.html

Convierte un JSON escapado (con `\"`, `\\n`, `\\t`, etc.) a un JSON formateado y legible, con resaltado de sintaxis.

**¿Cuándo usarla?**
Cuando recibes un payload como string escapado desde logs, Anypoint, Postman o una respuesta de API y necesitas leerlo rápidamente.

**Funcionalidades:**
- Tres estrategias de parsing automático (JSON directo, unescape manual, string envuelto en comillas)
- Resaltado de sintaxis por tipo de dato (strings, números, booleanos, null)
- Botón para copiar el resultado al portapapeles
- Botón para descargar el resultado como archivo `.json`
- Atajo de teclado: `Ctrl+Enter` / `Cmd+Enter` para convertir

---

### 2. JSON Diff
**Archivo:** `json-diff.html`
**URL:** https://ferchounisangil.github.io/Mulesoft-tools/json-diff.html

Compara dos JSONs campo por campo y resalta visualmente todas las diferencias, incluyendo objetos anidados y arrays.

**¿Cuándo usarla?**
Cuando necesitas comparar el payload de entrada vs. salida de un flujo, validar transformaciones DataWeave, o detectar qué cambió entre dos respuestas de API.

**Funcionalidades:**
- Comparación recursiva (objetos anidados, arrays)
- Diferencias resaltadas por tipo:
  - 🟡 **Modificado** — el campo existe en ambos pero con distinto valor
  - 🟢 **Agregado** — campo nuevo en el JSON B
  - 🔴 **Eliminado** — campo que solo existe en el JSON A
  - ⬜ **Igual** — campo idéntico en ambos
- Resumen con conteo de diferencias por tipo
- Filtros rápidos para ver solo un tipo de diferencia
- Búsqueda por nombre de campo en tiempo real
- Botón para intercambiar JSON A ↔ B
- Atajo de teclado: `Ctrl+Enter` / `Cmd+Enter` para comparar

---

## 🚀 Uso local

Clona el repositorio y abre cualquier archivo `.html` directamente en el navegador:

```bash
git clone https://github.com/ferchounisangil/Mulesoft-tools.git
cd Mulesoft-tools
open json-unescape.html   # macOS
open json-diff.html
```

No requiere servidor, Node.js ni ninguna dependencia externa.

---

## 👤 Autor

Equipo MuleSoft — **Suratech Insurtech / Tecnología**
