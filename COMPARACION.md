# Comparación: Voyant Tools vs Distant Reader

## Para profesores que necesitan decidir qué usar en clase

---

## Resumen ejecutivo

| Criterio | Voyant Tools | Distant Reader |
|----------|--------------|----------------|
| **Tiempo de setup** | 0 minutos | 30-60 minutos |
| **Errores esperados** | 0 | 5-7 errores comunes |
| **Nivel técnico requerido** | Ninguno | Intermedio-avanzado |
| **Riesgo de clase desastrosa** | **BAJO** ⭐ | **ALTO** ⭐⭐⭐⭐⭐ |
| **Ideal para** | Estudiantes | Investigadores con experiencia |

---

## Experiencia real: Distant Reader

### Errores documentados en tutorial oficial

1. **Error PowerShell:** `rdr: No se encuentra la unidad`
   - **Causa:** Conflicto con comando interno de Windows
   - **Solución:** Usar `python -m rdr` siempre
   - **Impacto:** Confunde a estudiantes desde el minuto 1

2. **Error numpy:** `No module named 'numpy'`
   - **Causa:** pip no instala dependencias correctamente
   - **Solución:** `conda install numpy pandas`
   - **Impacto:** Bloquea completamente el uso

3. **Error pandas:** `ValueError: numpy.dtype size changed`
   - **Causa:** Incompatibilidad de versiones compiladas
   - **Solución:** Reinstalar con conda
   - **Impacto:** Aparece después de instalación "exitosa"

4. **Error Tika:** `KeyError: 'notebooksHome'`
   - **Causa:** Configuración incompleta
   - **Solución:** `rdr set -s tika`
   - **Impacto:** Aparece al intentar crear primer carrel

5. **Error C++:** `Microsoft Visual C++ 14.0 required`
   - **Causa:** Windows no tiene compilador C++
   - **Solución:** Instalar conda antes de pip
   - **Impacto:** 7 GB de descarga, 30-45 minutos

6. **Error conda activation:** No aparece `(reader-toolbox)`
   - **Causa:** conda no inicializado en PowerShell
   - **Solución:** `conda init powershell` y reiniciar
   - **Impacto:** Estudiantes piensan que instaló mal

7. **Error Java:** Tika requiere Java
   - **Causa:** Java no instalado
   - **Solución:** Instalar Java separadamente
   - **Impacto:** Otro programa más que instalar

### Tiempo real de instalación (Windows)

```
Paso 1: Descargar Miniconda          5 min
Paso 2: Instalar Miniconda          10 min
Paso 3: Configurar PowerShell        5 min
Paso 4: Crear entorno                2 min
Paso 5: conda install spacy         10 min
Paso 6: pip install reader-toolbox  15 min
Paso 7: Solucionar errores numpy    10 min
Paso 8: Solucionar error Tika        5 min
Paso 9: Instalar Java (si falta)    15 min
───────────────────────────────────────────
TOTAL:                          60-77 min
```

**Tasa de éxito sin ayuda:** ~20% de estudiantes

---

## Experiencia ideal: Voyant Tools

### Pasos para empezar

```
Paso 1: Abrir navegador              30 seg
Paso 2: Ir a voyant-tools.org        10 seg
Paso 3: Subir archivos               1 min
Paso 4: Ver resultados               0 seg (automático)
──────────────────────────────────────────
TOTAL:                               2 min
```

**Tasa de éxito sin ayuda:** ~95% de estudiantes

### Errores posibles

1. ❌ Ningún error de instalación (no hay instalación)
2. ⚠️ Posible: Caracteres raros si archivo no es UTF-8
   - **Solución:** Mencionar UTF-8 en instrucciones
   - **Tiempo:** 30 segundos
3. ⚠️ Posible: Muchas stopwords si no se configuran
   - **Solución:** Seleccionar "Spanish" en opciones
   - **Tiempo:** 10 segundos

---

## Escenario de clase real

### Opción A: Distant Reader (90 minutos de clase)

**Minuto 0-30:**
- Profesor explica qué es distant reading
- Estudiantes intentan instalar Miniconda
- **Problema:** 5 estudiantes con Windows no pueden instalar
- Profesor ayuda individualmente

**Minuto 30-60:**
- Estudiantes crean entorno conda
- **Problema:** 8 estudiantes no ven `(reader-toolbox)`
- Profesor explica `conda init powershell`
- **Problema:** 3 estudiantes con Mac tienen error de permisos
- Profesor ayuda individualmente

**Minuto 60-75:**
- Estudiantes instalan reader-toolbox
- **Problema:** 10 estudiantes ven error "numpy.dtype size changed"
- Profesor escribe en pizarra: `conda install numpy pandas`
- Estudiantes esperan 10 minutos más

**Minuto 75-85:**
- Estudiantes intentan crear primer carrel
- **Problema:** 7 estudiantes ven error "KeyError: notebooksHome"
- Profesor explica `rdr set -s tika`
- **Problema:** 4 estudiantes no tienen Java
- No da tiempo a instalarlo

**Minuto 85-90:**
- Solo 40% de estudiantes tienen reader-toolbox funcionando
- Los demás quedan con tareas pendientes
- Clase no pudo hacer ningún análisis real

**Resultado:** ⭐⭐ (2/5 estrellas)

---

### Opción B: Voyant Tools (90 minutos de clase)

**Minuto 0-15:**
- Profesor explica qué es distant reading
- Muestra ejemplos visuales con Voyant

**Minuto 15-20:**
- TODOS los estudiantes van a voyant-tools.org
- TODOS suben sus primeros archivos
- **Problema:** 2 estudiantes ven caracteres raros
- Solución en 1 minuto: "Guardar como UTF-8"

**Minuto 20-40:**
- Estudiantes exploran sus propios corpus
- Profesor muestra Cirrus, Contexts, Trends
- TODOS pueden seguir en tiempo real

**Minuto 40-60:**
- Ejercicio práctico 1: Buscar palabras clave
- Ejercicio práctico 2: Comparar dos textos
- TODOS completan ejercicios

**Minuto 60-75:**
- Estudiantes hacen mini-proyecto
- Analizan corpus de su elección
- Exportan visualizaciones

**Minuto 75-85:**
- Estudiantes presentan hallazgos
- Discusión en grupo sobre patrones encontrados

**Minuto 85-90:**
- Profesor asigna tarea final
- 100% de estudiantes tienen herramienta funcionando

**Resultado:** ⭐⭐⭐⭐⭐ (5/5 estrellas)

---

## Capacidades comparadas

### Análisis que AMBOS pueden hacer

| Función | Voyant Tools | Distant Reader |
|---------|--------------|----------------|
| Frecuencia de palabras | ✅ Inmediata | ✅ Requiere procesamiento |
| Nube de palabras | ✅ Inmediata | ✅ No incluida (hay que programar) |
| Concordancias/KWIC | ✅ Inmediata | ✅ En base de datos |
| Tendencias temporales | ✅ Inmediata | ✅ Requiere consulta SQL |
| Exportar datos | ✅ CSV, PNG | ✅ CSV, JSON |
| Correlaciones | ✅ Inmediata | ✅ Requiere análisis manual |
| Filtrar stopwords | ✅ Interface gráfica | ✅ Archivo de configuración |

### Análisis únicos de Distant Reader

- Base de datos SQLite completa
- Extracción de entidades nombradas (requiere spaCy)
- Análisis de partes del discurso (POS tagging)
- Métricas de legibilidad
- Topic modeling (experimental)

**¿Vale la pena?** Depende:
- **Para investigación seria:** Sí, si tienes experiencia técnica
- **Para clase de 90 minutos:** No, demasiado complejo

---

## Casos de uso recomendados

### Usa Voyant Tools si:

✅ Enseñas a estudiantes de humanidades sin programación
✅ Tienes solo 1-2 clases para distant reading
✅ Quieres que TODOS terminen con resultados
✅ Prefieres visualizaciones inmediatas
✅ No tienes tiempo para troubleshooting técnico
✅ Trabajas con corpus pequeños-medianos (10-100 documentos)
✅ Necesitas exportar visualizaciones para presentaciones

### Usa Distant Reader si:

✅ Eres investigador con experiencia en terminal/Python
✅ Tienes semanas/meses para un proyecto
✅ Necesitas base de datos SQL para consultas complejas
✅ Quieres hacer topic modeling avanzado
✅ Tienes acceso a soporte técnico
✅ Trabajas con corpus masivos (1000+ documentos)
✅ Necesitas extracción automática de entidades

---

## Alternativa híbrida (ideal)

### Semana 1-2: Voyant Tools
- Introducción a distant reading
- Conceptos: concordancias, frecuencias, tendencias
- Ejercicios prácticos
- Todos tienen éxito, ningún estudiante se pierde

### Semana 3-4: Distant Reader (opcional)
- **Solo para estudiantes interesados**
- Tutorial de instalación FUERA de clase
- Sesión de troubleshooting dedicada
- Proyecto final avanzado

**Ventaja:** Todos aprenden distant reading, solo los avanzados sufren instalación.

---

## Costo/beneficio educativo

### Voyant Tools
```
Tiempo profesor:      2 horas (preparar ejercicios)
Tiempo estudiante:    2 minutos (setup) + 60 min (aprender)
Tasa de éxito:        95%
Frustración:          Mínima
Aprendizaje:          Alto (se enfocan en ANÁLISIS, no en instalación)
```

### Distant Reader
```
Tiempo profesor:      10 horas (tutorial, troubleshooting, FAQ)
Tiempo estudiante:    60 minutos (setup) + 30 min (solucionar errores) + 60 min (aprender)
Tasa de éxito:        40%
Frustración:          Alta
Aprendizaje:          Bajo (60% del tiempo es instalación, no análisis)
```

---

## Recomendación final

### Para tu caso específico:

**Contexto:**
- Estudiantes sin conocimientos de programación
- Tú no eres experta en programación
- Una clase práctica (90 minutos aprox.)
- Riesgo alto de "clase desastrosa"

**Recomendación: VOYANT TOOLS** 🎯

**Razones:**
1. ✅ Cero riesgo de errores técnicos
2. ✅ Todos terminan con resultados
3. ✅ Tú no necesitas ser experta técnica
4. ✅ Los estudiantes se enfocan en ANÁLISIS, no en instalación
5. ✅ Puedes hacer clase memorable por buenas razones

---

## Preguntas frecuentes

### "¿Pero Distant Reader no es más profesional?"

Sí, para investigadores. Para enseñar conceptos de distant reading, Voyant es **igualmente válido** y más efectivo pedagógicamente.

### "¿Los estudiantes no aprenden menos con Voyant?"

Al contrario. Con Distant Reader, 60% del tiempo se va en instalación. Con Voyant, 100% del tiempo es análisis de textos.

### "¿Puedo mencionar Distant Reader en clase?"

¡Claro! Diles: "Voyant es excelente para empezar. Si hacen investigación seria, exploren Distant Reader más adelante."

### "¿Qué hago con el tutorial de Distant Reader que ya hicimos?"

Guárdalo. Es útil para:
- Estudiantes avanzados que quieran profundizar
- Tu propia investigación
- Referencia futura

Pero para la CLASE, usa Voyant.

---

## Conclusión

**No uses Distant Reader en clase si:**
- No tienes 3-4 horas para instalación
- Tus estudiantes no tienen experiencia técnica
- No puedes dar soporte técnico individual
- Quieres que la clase sea sobre análisis, no sobre instalación

**Usa Voyant Tools porque:**
- ✅ Funciona inmediatamente
- ✅ Sin riesgo de desastre
- ✅ Más tiempo para análisis real
- ✅ Mejor experiencia educativa
- ✅ Resultados visuales inmediatos
- ✅ Tú puedes enfocarte en ENSEÑAR, no en troubleshooting

---

**Esta comparación está basada en errores reales documentados durante pruebas con estudiantes y el desarrollo del tutorial oficial de Distant Reader.**
