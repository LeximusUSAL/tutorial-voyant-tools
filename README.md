# Tutorial: Análisis de Textos con Voyant Tools

## Guía completa para principiantes (sin programación)

---

## ¿Qué es Voyant Tools?

**Voyant Tools** es una herramienta web **gratuita** para analizar textos de forma visual. No necesitas instalar nada, funciona directamente en tu navegador.

**Ventajas:**
- ✅ **100% en línea** - no hay que instalar programas
- ✅ **Gratis** - sin límites de uso
- ✅ **Visual** - gráficos y nubes de palabras automáticas
- ✅ **Funciona en español** - reconoce textos en cualquier idioma
- ✅ **Sin errores** - subes tus archivos y funciona inmediatamente

---

## Requisitos

- Computadora con navegador web (Chrome, Firefox, Safari, Edge)
- Conexión a Internet
- Tus archivos de texto (.txt) o PDFs

**No necesitas:**
- ❌ Python
- ❌ Programación
- ❌ Conocimientos técnicos
- ❌ Instalaciones complicadas

---

## PASO 1: Preparar tus archivos

### 1.1. Organiza tus documentos

Crea una carpeta en tu escritorio con todos los archivos que quieres analizar.

**Formatos aceptados:**
- Archivos de texto plano (.txt) ← **Recomendado**
- PDF
- Word (.doc, .docx)
- HTML
- XML

**Tip:** Si tienes PDFs, lo ideal es convertirlos primero a .txt para mejores resultados.

---

### 1.2. Convertir PDF a TXT (opcional pero recomendado)

Si tus documentos son PDFs, conviértelos a .txt primero:

#### **Opción A: Usando un convertidor online (MÁS FÁCIL)**

1. Ve a: https://www.ilovepdf.com/es/pdf_a_texto
2. Sube tu PDF
3. Haz clic en "Convertir a TXT"
4. Descarga el archivo .txt
5. Repite para cada PDF

#### **Opción B: Usando pdfminer (si ya lo tienes instalado)**

```bash
# Mac/Linux
pdf2txt.py archivo.pdf -o archivo.txt

# Windows
pdf2txt.py archivo.pdf -o archivo.txt
```

---

## PASO 2: Abrir Voyant Tools

### 2.1. Ir al sitio web

1. Abre tu navegador web
2. Ve a: **https://voyant-tools.org**
3. Verás la página principal con un cuadro de texto grande

**¡Eso es todo! Ya estás listo para empezar.**

---

## PASO 3: Subir tus archivos a Voyant

Tienes **3 formas** de subir tus textos:

### **Método 1: Subir archivos desde tu computadora (RECOMENDADO)**

1. Haz clic en el botón **"Subir"** (o "Upload")
2. Selecciona uno o varios archivos de tu computadora
3. Haz clic en **"Abrir"**
4. Haz clic en el botón azul **"Revelar"** (o "Reveal")
5. **¡Espera 5-30 segundos mientras procesa!**
6. ✅ Verás tu análisis con gráficos

**Puedes subir:**
- Un solo archivo
- Múltiples archivos a la vez (Ctrl+Click o Cmd+Click) o en carpeta comprimida ZIP (más sencillo)
- Hasta 10 MB por archivo

---

### **Método 2: Pegar texto directamente**

1. Copia un texto de cualquier lugar (Word, PDF, página web)
2. Pégalo en el cuadro de texto grande de la página principal
3. Haz clic en **"Revelar"**
4. ✅ Análisis inmediato

---

### **Método 3: Usar una URL**

1. Si tu texto está en una página web, copia la URL
2. Pégala en el cuadro de texto
3. Haz clic en **"Revelar"**
4. Voyant descargará y analizará automáticamente

---

## PASO 4: Entender la interfaz de Voyant

Cuando subes tus textos, verás **5 paneles principales**:

```
┌─────────────────┬─────────────────┐
│    CIRRUS       │    READER       │
│ (nube palabras) │ (lector texto)  │
├─────────────────┼─────────────────┤
│    TRENDS       │   SUMMARY       │
│  (tendencias)   │   (resumen)     │
├─────────────────┴─────────────────┤
│         CONTEXTS                  │
│        (contextos)                │
└───────────────────────────────────┘
```

### **Panel 1: Cirrus (nube de palabras)**
- Muestra las palabras más frecuentes en tamaño grande
- Palabras más grandes = más frecuentes
- Haz clic en una palabra para ver dónde aparece

### **Panel 2: Reader (lector)**
- Muestra el texto completo
- Palabras destacadas = palabras frecuentes
- Puedes navegar entre documentos

### **Panel 3: Trends (tendencias)**
- Gráfico de líneas mostrando frecuencia de palabras a lo largo del corpus
- Útil para ver evolución de términos

### **Panel 4: Summary (resumen)**
- Estadísticas del corpus:
  - Total de palabras
  - Palabras únicas
  - Densidad del vocabulario
  - Palabras más frecuentes

### **Panel 5: Contexts (contextos)**
- Muestra palabras en su contexto (concordancias)
- Útil para análisis cualitativo

---

## PASO 5: Herramientas principales de Voyant

### 5.1. **Cirrus (Nube de palabras)**

**Para qué sirve:** Visualización rápida de términos frecuentes

**Cómo usarlo:**
1. Observa las palabras más grandes
2. Haz clic en cualquier palabra para ver detalles
3. **Opciones del panel:**
   - 🔧 Haz clic en el icono de herramienta (esquina superior derecha)
   - Cambia cantidad de términos mostrados
   - Exporta la imagen

**Tips:**
- Palabras vacías (stopwords) como "el", "la", "de" se filtran automáticamente
- Puedes añadir tus propias stopwords si quieres filtrar más palabras

---

### 5.2. **Terms (Términos)**

**Para qué sirve:** Ver lista de palabras ordenadas por frecuencia

**Cómo acceder:**
1. Haz clic en cualquier panel
2. Busca los iconos pequeños arriba a la derecha
3. Haz clic en el icono de "ventanas" y selecciona **"Terms"**

**Verás una tabla con:**
- Palabra
- Frecuencia (count)
- Frecuencia relativa
- Tendencia

**Puedes:**
- Ordenar por frecuencia
- Buscar palabras específicas
- Exportar la lista a Excel

---

### 5.3. **Contexts (Concordancias/KWIC)**

**Para qué sirve:** Ver palabras en su contexto real

**Cómo usarlo:**
1. Escribe una palabra en el cuadro de búsqueda del panel Contexts
2. Verás todas las veces que aparece con contexto antes y después
3. Haz clic en cualquier línea para ir al documento completo

**Ejemplo:**
```
...en el teatro de la    ópera    se presentó una nueva...
...la mejor cantante de  ópera    que he escuchado...
...programación de       ópera    italiana en Madrid...
```

---

### 5.4. **Trends (Tendencias)**

**Para qué sirve:** Ver cómo cambia el uso de palabras a lo largo del corpus

**Cómo usarlo:**
1. Escribe palabras clave en el cuadro de búsqueda
2. Verás líneas de colores mostrando frecuencia en cada documento
3. Útil si tus documentos están en orden cronológico

**Ejemplo de uso:**
- Comparar "piano" vs "guitarra" en revistas musicales
- Ver evolución de "jazz" vs "ópera" a lo largo del tiempo

---

### 5.5. **Correlations (Correlaciones)**

**Para qué sirve:** Encontrar palabras que aparecen juntas frecuentemente

**Cómo acceder:**
1. Cambiar un panel a "Correlations"
2. Selecciona un término
3. Verás qué palabras aparecen frecuentemente cerca de ese término

**Ejemplo:**
- Término: "piano"
- Correlaciones: "concierto", "compositor", "sonata", "solista"

---

## PASO 6: Funciones avanzadas (opcional)

### 6.1. **Filtrar palabras vacías (stopwords)**

Si quieres eliminar palabras específicas del análisis:

1. Haz clic en **"Options"** (esquina superior derecha, al lado de "Revelar")
2. Marca **"Edit List"** en "Stopwords"
3. **Selecciona idioma:** Spanish
4. **Añade palabras personalizadas:** Una por línea
5. Haz clic en **"Confirm"**

---

### 6.2. **Exportar resultados**

Puedes exportar tus visualizaciones:

1. En cualquier panel, haz clic en el icono **"Export"** (esquina superior derecha)
2. **Opciones:**
   - **Export Visualization:** Guarda como imagen (PNG)
   - **Export Data:** Guarda datos como CSV (abre en Excel)
   - **Export URL:** Guarda enlace para compartir tu análisis

**Importante:** La URL de exportación te permite **compartir tu análisis completo** con otros. Guárdala si quieres volver más tarde.

---

### 6.3. **Guardar tu trabajo**

Voyant **NO guarda automáticamente**. Para guardar:

**Opción 1: Guardar la URL**
1. Copia la URL de tu navegador
2. Guárdala en un documento
3. Puedes volver a ella cuando quieras

**Opción 2: Exportar datos**
1. Exporta cada panel como CSV o imagen
2. Guarda en tu computadora

---

## PASO 7: Ejemplos de uso académico

### Ejemplo 1: Analizar Bibliografía para tus investigaciones

**Objetivo:** Encontrar patrones y tendencias

**Pasos:**
1. Sube archivos .txt con bibliografía seleccionada
2. Observa Cirrus: verás las palabras y conceptos más utilizados
3. Usa Contexts para ver cómo usa "nacionalismo" o "españa" los distintos textos
4. Usa Correlations para encontrar palabras asociadas a "española"

---

### Ejemplo 2: Comparar dos autores

**Objetivo:** Comparar vocabulario de textos de musicología de 1910 vs. un texto de 2024

**Pasos:**
1. Sube textos de las dos épocas marcando en el nombre del archivo en primer lugar el año de publicación
2. Usa Terms para ver palabras más frecuentes de cada uno
3. Usa Trends para ver qué palabras son únicas de cada autor
4. Exporta tablas para comparar en Excel

---

### Ejemplo 3: Análisis de revistas musicales

**Objetivo:** Estudiar evolución del lenguaje musical

**Pasos:**
1. Sube revistas en orden cronológico (nombra archivos: 1900_revista.txt, 1910_revista.txt)
2. Usa Trends para ver evolución de "jazz", "ópera", "radio"
3. Usa Contexts para ver contextos de "compositor" vs "intérprete"
4. Usa Summary para comparar vocabulario entre décadas

---

## PASO 8: Consejos y mejores prácticas

### ✅ HACER:

- **Nombres de archivo claros:** `1920_revista_musical.txt` mejor que `doc1.txt`
- **Orden cronológico:** Si estudias evolución temporal, nombra archivos con fechas
- **Limpiar textos:** Elimina encabezados, pies de página, números de página antes de subir
- **UTF-8:** Asegúrate de que archivos .txt estén en codificación UTF-8
- **Probar primero:** Sube 2-3 archivos de prueba antes de subir todo el corpus

### ❌ EVITAR:

- **Archivos muy grandes:** Si un archivo tiene +10 MB, divídelo
- **Mezclar idiomas:** Procesa cada idioma por separado
- **PDFs escaneados:** No funcionan bien (necesitan OCR primero)
- **Textos sin limpiar:** Manteles, índices, publicidad distorsionan resultados

---

## PASO 9: Solución de problemas

### Problema 1: "El análisis tarda mucho"

**Solución:**
- Archivos muy grandes (>5 MB) tardan más
- Divide archivos grandes en partes más pequeñas
- Ten paciencia: corpus de 100+ documentos puede tardar 1-2 minutos

---

### Problema 2: "Veo muchas palabras vacías (el, la, de, que)"

**Solución:**
1. Haz clic en **"Options"** al subir archivos
2. Asegúrate de seleccionar **"Spanish"** en Stopwords
3. Si aún ves palabras no deseadas, añádelas manualmente en "Edit List"

---

### Problema 3: "Los caracteres españoles (á, é, í, ñ) no se ven bien"

**Solución:**
- Asegúrate de que tus archivos .txt estén guardados en **UTF-8**
- En Windows: Notepad → "Guardar como" → Codificación: UTF-8
- En Mac: TextEdit → Formato → Codificar como → UTF-8

---

### Problema 4: "Quiero analizar PDFs pero no funcionan bien"

**Solución:**
1. Convierte PDFs a .txt primero
2. Usa https://www.ilovepdf.com/es/pdf_a_texto
3. Sube los archivos .txt resultantes

**PDFs escaneados (imágenes):**
- Necesitas OCR (reconocimiento óptico)
- Usa: https://www.onlineocr.net/es/
- Luego convierte a .txt

---

## PASO 10: Recursos adicionales

### Documentación oficial
- **Documentación completa:** https://voyant-tools.org/docs/#!/guide/start
- **Videos tutoriales:** https://www.youtube.com/results?search_query=voyant+tools+tutorial
- **Ejemplos:** https://voyant-tools.org/docs/#!/guide/examples

### Tutoriales en español
- Tutorial básico: https://programminghistorian.org/es/lecciones/analisis-voyant-tools
- Guía digital humanities: https://hdlab.space/Voyant-Tools/

### Comunidad
- Foro de Voyant: https://github.com/voyanttools/Voyant/discussions
- Twitter: @VoyantTools

---

## PASO 11: Actividad práctica para estudiantes

### Ejercicio: Análisis de bibliografía para tu investigación

**Objetivo:** Familiarizarse con Voyant Tools en 30 minutos

**Materiales:**
- 10 artículos en español (.txt)
- Computadora con Internet

**Actividad paso a paso:**

1. **[5 min] Preparación:**
   - Pasar tus artículos en .pdf a .txt
   - Guardarlos como .txt

2. **[5 min] Subir a Voyant:**
   - Ir a https://voyant-tools.org
   - Subir los archivos txt
   - Hacer clic en "Revelar"

3. **[10 min] Exploración:**
   - Observar Cirrus: ¿Cuáles son las 10 palabras más frecuentes?
   - Ver Summary: ¿Cuántas palabras tiene el corpus?
   - Buscar en Contexts la palabra "española"

4. **[10 min] Análisis:**
   - Usar Trends para comparar "española" vs "universal"
   - Usar Correlations para encontrar palabras asociadas a "Música"
   - Exportar nube de palabras como imagen

5. **[5 min] Reflexión:**
   - ¿Qué palabras clave son las principales en tu bibliografía seleccionada?
   - ¿Qué patrones encontraste?

---

## Conclusión

**Voyant Tools es ideal para:**
- ✅ Clases de humanidades digitales / Investigación en Musicología
- ✅ Análisis estilo en distintas épocas históricas
- ✅ Estudios de corpus
- ✅ Análisis de prensa histórica
- ✅ Investigación exploratoria
- ✅ Estudiantes sin conocimientos técnicos

**No necesitas:**
- ❌ Programación
- ❌ Python
- ❌ Instalaciones complejas
- ❌ Conocimientos de terminal

**Tiempo total de aprendizaje:** 15-30 minutos

**¡Empieza ahora:** https://voyant-tools.org

---

## Preguntas frecuentes

### ¿Es realmente gratis?
Sí, 100% gratis sin límites de uso.

### ¿Mis textos quedan públicos?
No. Tus textos no se publican automáticamente. Solo si compartes la URL del análisis.

### ¿Puedo usar Voyant sin Internet?
No, Voyant es una herramienta web. Pero existe Voyant Server (versión para instalar localmente) si necesitas trabajar offline.

### ¿Hay límite de archivos?
No hay límite estricto, pero corpus muy grandes (+100 MB) pueden tardar mucho. Lo ideal: 10-50 archivos de tamaño medio.

### ¿Puedo analizar textos en otros idiomas?
Sí, Voyant funciona con cualquier idioma. Tiene stopwords para: inglés, francés, alemán, italiano, español, portugués, y más.

### ¿Puedo descargar Voyant?
Sí, existe Voyant Server para instalar en tu computadora, pero para uso educativo la versión web es suficiente.

---

**Creado para estudiantes del Máster en Música Hispana.**

Proyecto LexiMus: Léxico y Ontología de la Música en Español (Universidad de Salamanca) Prensa musical e Inteligencia Artificial. Proyecto LexiMus: Léxico y ontología de la música en español (PID2022-139589NB-C33), Universidad de Salamanca. Disponible en: https://LeximusUSAL.github.io/inicio
© 2025 Universidad de Salamanca

**Última actualización:** Enero 2025
