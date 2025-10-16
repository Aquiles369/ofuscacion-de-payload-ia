# Release Notes — v1.0.0 (2025-10-14)

## 🧠 Resumen
**Promt de IA + Ofuscación de payload** es un generador avanzado de variantes XSS que transforma strings e identificadores sin romper la ejecución ni la sintaxis original.  
Ideal para probar bypasses contra WAF modernos, validar filtros y entrenar laboratorios con payloads realistas.

📺 Demo disponible en YouTube.

---

## 🧪 Problema que resuelve
- ❌ Los payloads XSS tradicionales son detectados fácilmente por WAF y sanitizadores.
- ❌ La mayoría de herramientas no generan variantes funcionales, rompiendo ejecución.
- ❌ Falta de reproducibilidad: resultados distintos cada vez.

✅ Esta herramienta resuelve todo eso creando variantes **funcionales, ofuscadas y reproducibles**, sin alterar la lógica del payload original.

---

## ⚙️ Qué aporta y cómo beneficia
- 🧬 **Ofuscación profunda:** aplica bloques Unicode (ASCII, Greek, Cyrillic, Math, etc.) para evadir filtros sin romper ejecución.
- 🔁 **Variantes únicas por payload:** controladas por `variants_per_payload`.
- 🎯 **Seed opcional:** garantiza que el mismo input siempre produzca el mismo output.
- 🛡️ **Bypass real:** técnicas de sustitución, homoglifos y manipulación carácter por carácter.
- 🧪 **Laboratorio realista:** prueba contra WAF, parsers y validadores avanzados.
- 🤖 **Automatización total:** ingresá un payload y obtené cientos o miles de variantes listas.

---

## 🧰 Características principales

### 📥 Inputs del usuario
- Payload único o lista de payloads.
- `seed` para reproducibilidad.
- `variants_per_payload` para definir cuántas variantes generar.
- `x17_blocks` para elegir bloques Unicode.
- `modo_validación` (`estricto` o `relajado`).
- Flags opcionales: `#*`, `#**`, `#a`.

---

### ⚙️ Validación estricta (checks A–E)
- ✅ Tokens críticos preservados.
- ✅ Balanceo de paréntesis/comillas/corchetes.
- ✅ Primitiva de ejecución presente (alert/confirm/onerror).
- ✅ Sin invisibles/BIDI disruptivos.
- ✅ Bloques Unicode válidos.

Si un payload falla → se descarta y regenera (máx. 3 intentos).

---

## 📦 Formato de salida
- 📤 Solo la lista de payloads generados, uno por línea.
- ❌ Sin metadatos, hashes o información adicional.

---

## 🛠️ Casos de uso
- 🧪 Laboratorios de seguridad web.
- ⚔️ Investigación de bypasses de WAF.
- 🧠 Entrenamiento avanzado en XSS.
- 🤖 Automatización de pruebas ofensivas con IA.

---

## 🛣️ Roadmap
- ✅ Versión inicial con soporte para 28 bloques Unicode.
- ⏭️ Próxima versión: soporte extendido a codificaciones mixtas + generación automática basada en contexto.

---

**“Camuflaje quirúrgico para tus XSS: invisible al WAF, letal en ejecución.”**
