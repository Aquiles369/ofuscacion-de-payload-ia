# Política de seguridad

## 🧠 Resumen
**Promt de IA + Ofuscación de payload** es una herramienta educativa y de investigación ofensiva para entornos controlados.  
No ejecuta código ni explota sistemas por sí sola. Su propósito es generar variantes ofuscadas de payloads para pruebas de seguridad en laboratorios y programas de bug bounty autorizados.

---

## 🔐 Principios de seguridad

- ✅ **Uso ético y legal:** solo debe emplearse en entornos controlados, laboratorios y programas de bug bounty con autorización explícita.
- 🧪 **Contenido seguro:** no incluye payloads maliciosos activos ni exploits reales.
- ⚙️ **Transformación local:** el proceso de ofuscación ocurre sin llamadas externas ni recopilación de datos.
- 🧠 **No persistencia:** no almacena datos sensibles del usuario ni registra payloads generados.

---

## ✅ Buenas prácticas recomendadas

- Usar exclusivamente en entornos de laboratorio o en sistemas donde tengas permiso para realizar pruebas.  
- Revisar cada variante generada antes de usarla en auditorías reales.  
- Mantener logs internos para trazabilidad y análisis de resultados.  
- Evitar el uso en sistemas productivos sin autorización.

---

## 🐛 Reporte de problemas

Si detectás comportamientos inesperados, falsos positivos o variantes incorrectas:

1. No compartas payloads sensibles públicamente.  
2. Reportá el problema vía issues en GitHub o por Discord.  
3. Incluí el payload original, flags usados, bloques seleccionados y resultado obtenido.

---

## 🛡️ Alcance de seguridad

| Área                        | Estado                       |
|----------------------------|-----------------------------|
| Backend / API              | ❌ No aplica                |
| Ejecución de código       | ❌ No incluida             |
| Payloads activos          | ❌ No incluidos            |
| Generador de variantes    | ✅ Incluido               |
| Datos sensibles           | ❌ No deben almacenarse    |

---

## ⚠️ Descargo
Este proyecto tiene fines educativos y de investigación.  
El uso indebido de la herramienta o sus resultados puede ser ilegal.  
El autor no se hace responsable por acciones no autorizadas derivadas de su uso.

---

**“Camuflaje quirúrgico para tus XSS: invisible al WAF, letal en ejecución.”**
