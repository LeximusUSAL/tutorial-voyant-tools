# Tutorial: Análisis de Textos con AntConc

## Guía completa para principiantes (Mac y Windows)

---

## ¿Qué es AntConc?

**AntConc** es un programa gratuito para análisis de corpus lingüístico. Es una herramienta de escritorio (se instala en tu computadora) creada por Laurence Anthony de la Universidad de Waseda.

**Ventajas:**
- ✅ **Instalación simple** - Un solo archivo, sin dependencias
- ✅ **Gratuito** - 100% gratis
- ✅ **Sin Internet** - Funciona offline
- ✅ **Rápido** - Procesa miles de archivos localmente
- ✅ **Concordancias potentes** - Especializado en análisis KWIC
- ✅ **Funciona en español** - Compatible con UTF-8

**Desventajas comparado con Voyant:**
- ❌ Interfaz menos visual (sin nubes de palabras)
- ❌ Requiere descarga e instalación
- ❌ Curva de aprendizaje más técnica

---

## Requisitos

### Para Mac:
- MacOS 10.10 o superior
- Procesador Intel o Apple Silicon (M1/M2/M3)
- 50 MB de espacio en disco

### Para Windows:
- Windows 7 o superior (Windows 10/11 recomendado)
- 50 MB de espacio en disco

### Para ambos sistemas:
- Tus archivos de texto en formato .txt (UTF-8)

---

## PASO 1: Descargar AntConc

### 1.1. Para Windows

1. **Abre tu navegador web** (Chrome, Edge, Firefox)

2. **Ve a la página oficial:**
   - URL: https://www.laurenceanthony.net/software/antconc/

3. **Descarga la versión para Windows:**
   - Busca la sección "Downloads"
   - Haz clic en **"AntConc 4.3.1 (Windows)"** (o versión más reciente)
   - Se descargará un archivo ZIP: `AntConc4.3.1_windows.zip`

4. **Espera a que termine la descarga**
   - Verás el archivo en tu carpeta de Descargas
   - Tamaño aproximado: 10-15 MB

---

### 1.2. Para Mac

1. **Abre tu navegador web** (Safari, Chrome, Firefox)

2. **Ve a la página oficial:**
   - URL: https://www.laurenceanthony.net/software/antconc/

3. **Descarga la versión correcta según tu Mac:**

   **Si tienes Mac con Apple Silicon (M1/M2/M3):**
   - Haz clic en **"AntConc 4.3.1 (Macintosh - Apple Silicon)"**
   - Se descargará: `AntConc4.3.1_macOS_apple_silicon.dmg`

   **Si tienes Mac Intel (anterior a 2020):**
   - Haz clic en **"AntConc 4.3.1 (Macintosh - Intel)"**
   - Se descargará: `AntConc4.3.1_macOS_intel.dmg`

   **¿No sabes qué Mac tienes?**
   - Haz clic en el menú  (Apple) → "Acerca de este Mac"
   - Si dice "Chip Apple M1/M2/M3" → Apple Silicon
   - Si dice "Procesador Intel" → Intel

4. **Espera a que termine la descarga**
   - Verás el archivo .dmg en tu carpeta de Descargas
   - Tamaño aproximado: 15-20 MB

---

## PASO 2: Instalar AntConc

### 2.1. Instalación en Windows

1. **Abre tu carpeta de Descargas**
   - Presiona `Windows + E` para abrir Explorador de archivos
   - Ve a "Descargas"

2. **Busca el archivo descargado:**
   - `AntConc4.3.1_windows.zip`

3. **Descomprime el archivo ZIP:**
   - Haz clic derecho en el archivo ZIP
   - Selecciona **"Extraer todo..."** o **"Extract all..."**
   - En la ventana que aparece, haz clic en **"Extraer"**
   - Se creará una carpeta llamada `AntConc4.3.1_windows`

4. **Mueve la carpeta al escritorio (opcional pero recomendado):**
   - Arrastra la carpeta extraída a tu Escritorio
   - Así será más fácil encontrarla

5. **Abre la carpeta:**
   - Verás un archivo llamado **`AntConc.exe`**
   - Este es el programa

6. **Crea un acceso directo (opcional):**
   - Haz clic derecho en `AntConc.exe`
   - Selecciona "Crear acceso directo"
   - Arrastra el acceso directo a tu Escritorio

**✅ ¡Listo! AntConc está instalado.**

---

### 2.2. Instalación en Mac

1. **Abre tu carpeta de Descargas**
   - Abre Finder
   - Ve a "Descargas"

2. **Busca el archivo descargado:**
   - `AntConc4.3.1_macOS_apple_silicon.dmg` o
   - `AntConc4.3.1_macOS_intel.dmg`

3. **Haz doble clic en el archivo .dmg**
   - Se montará una imagen de disco
   - Aparecerá una ventana con el icono de AntConc

4. **Arrastra AntConc a la carpeta Aplicaciones:**
   - Verás una ventana con dos iconos:
     - Icono de AntConc (izquierda)
     - Icono de carpeta "Applications" (derecha)
   - **Arrastra el icono de AntConc hacia la carpeta Applications**

5. **Espera a que se copie:**
   - Tardará 10-20 segundos

6. **Expulsa la imagen de disco:**
   - Haz clic derecho en el icono de disco montado (en el escritorio o Finder)
   - Selecciona "Expulsar"

7. **Abre Launchpad:**
   - Presiona F4 o abre Launchpad desde el Dock
   - Busca "AntConc"
   - Verás el icono de AntConc

**✅ ¡Listo! AntConc está instalado.**

---

## PASO 3: Abrir AntConc por primera vez

### 3.1. Abrir en Windows

1. **Ve a la carpeta donde está AntConc**
   - Si lo pusiste en el Escritorio: ve al Escritorio
   - Entra a la carpeta `AntConc4.3.1_windows`

2. **Haz doble clic en `AntConc.exe`**

3. **Si aparece advertencia de Windows Defender:**
   - Verás: "Windows protegió tu PC"
   - Haz clic en **"Más información"**
   - Luego haz clic en **"Ejecutar de todas formas"**
   - Esta advertencia aparece porque AntConc no tiene firma digital, pero es seguro

4. **Se abrirá AntConc:**
   - Verás una ventana con múltiples pestañas arriba
   - La interfaz es simple, en inglés

**✅ AntConc está funcionando.**

---

### 3.2. Abrir en Mac

1. **Abre Launchpad o ve a Aplicaciones**
   - Presiona F4 o ve a Finder → Aplicaciones

2. **Busca y haz clic en "AntConc"**

3. **Si aparece advertencia de seguridad:**
   - Verás: "AntConc no se puede abrir porque proviene de un desarrollador no identificado"
   - **No te preocupes, AntConc es seguro**
   - Haz clic en **"Aceptar"** para cerrar la advertencia

4. **Permitir que se abra:**
   - Abre **Preferencias del Sistema** (Menú  → Preferencias del Sistema)
   - Ve a **"Seguridad y Privacidad"**
   - En la pestaña **"General"**, verás un mensaje:
     - "Se bloqueó AntConc porque proviene de un desarrollador no identificado"
   - Haz clic en **"Abrir de todas formas"**
   - Confirma haciendo clic en **"Abrir"**

5. **AntConc se abrirá:**
   - Verás una ventana con múltiples pestañas arriba
   - La interfaz es simple, en inglés

**✅ AntConc está funcionando.**

---

## PASO 4: Preparar tus archivos de texto

### 4.1. Formato requerido

AntConc **solo funciona con archivos de texto plano (.txt)**.

**Archivos compatibles:**
- ✅ `.txt` (texto plano)

**Archivos NO compatibles directamente:**
- ❌ `.pdf` (necesitas convertir)
- ❌ `.docx` (necesitas convertir)
- ❌ `.doc` (necesitas convertir)

---

### 4.2. Convertir archivos a .txt

#### Si tienes archivos PDF:

**Opción 1: Convertidor online (más fácil)**
1. Ve a: https://www.ilovepdf.com/es/pdf_a_texto
2. Sube tu PDF
3. Haz clic en "Convertir a TXT"
4. Descarga el archivo .txt

**Opción 2: Usando pdfminer (si ya lo tienes instalado)**
```bash
pdf2txt.py archivo.pdf -o archivo.txt
```

#### Si tienes archivos Word (.docx):

1. Abre el documento en Microsoft Word
2. Ve a **Archivo → Guardar como**
3. En "Tipo de archivo", selecciona **"Texto sin formato (*.txt)"**
4. Haz clic en "Guardar"
5. Cuando pregunte por codificación, selecciona **"UTF-8"**

---

### 4.3. Organizar tus archivos

1. **Crea una carpeta para tu corpus:**
   - En tu Escritorio, crea una carpeta llamada `MiCorpus`
   - Pon todos tus archivos .txt dentro

2. **Nombres de archivo claros:**
   - ✅ Buenos: `1920_revista_musical.txt`, `cervantes_quijote.txt`
   - ❌ Malos: `doc1.txt`, `archivo.txt`, `texto123.txt`

3. **Codificación UTF-8 (IMPORTANTE):**
   - Asegúrate de que tus archivos estén en UTF-8
   - En Windows: Notepad → Guardar como → Codificación: UTF-8
   - En Mac: TextEdit → Formato → Codificar como → UTF-8

---

## PASO 5: Cargar archivos en AntConc

### 5.1. Abrir archivos

1. **Abre AntConc** (si no está abierto)

2. **Carga tus archivos:**

   **Opción A: Abrir un solo archivo**
   - Ve a **File → Open File(s)...**
   - O presiona `Ctrl + O` (Windows) o `Cmd + O` (Mac)
   - Navega a tu carpeta `MiCorpus`
   - Selecciona un archivo .txt
   - Haz clic en "Abrir"

   **Opción B: Abrir múltiples archivos**
   - Ve a **File → Open File(s)...**
   - Selecciona múltiples archivos con `Ctrl + Click` (Windows) o `Cmd + Click` (Mac)
   - Haz clic en "Abrir"

   **Opción C: Abrir una carpeta completa (recomendado)**
   - Ve a **File → Open Dir...**
   - Selecciona tu carpeta `MiCorpus`
   - Haz clic en "Seleccionar carpeta"
   - **AntConc cargará TODOS los archivos .txt de la carpeta automáticamente**

3. **Verificar que se cargaron:**
   - En la esquina inferior izquierda verás: "Corpus Files: X"
   - Donde X es el número de archivos cargados
   - Ejemplo: "Corpus Files: 25"

**✅ Tus archivos están listos para analizar.**

---

## PASO 6: Interfaz de AntConc (pestañas principales)

AntConc tiene **7 pestañas principales** en la parte superior:

```
┌──────────────────────────────────────────────────┐
│ Concordance │ Concordance Plot │ File View │ ... │
└──────────────────────────────────────────────────┘
```

### Pestañas disponibles:

1. **Concordance** - Concordancias KWIC (keyword in context)
2. **Concordance Plot** - Visualización gráfica de distribución
3. **File View** - Ver archivo completo
4. **Clusters/N-Grams** - Grupos de palabras frecuentes
5. **Collocates** - Palabras que aparecen cerca de otra
6. **Word List** - Lista de frecuencias
7. **Keyword List** - Palabras clave comparadas con corpus de referencia

---

## PASO 7: Análisis básico - Word List (Lista de frecuencias)

### 7.1. Generar lista de palabras

1. **Haz clic en la pestaña "Word List"**

2. **Haz clic en el botón "Start"** (esquina inferior izquierda)

3. **Espera unos segundos** mientras AntConc procesa

4. **Verás tres columnas:**
   - **Rank** - Posición por frecuencia (1 = más frecuente)
   - **Freq** - Frecuencia (número de veces que aparece)
   - **Word** - La palabra

**Ejemplo:**
```
Rank  Freq   Word
1     1523   de
2     1204   la
3     892    el
4     654    en
5     543    y
```

---

### 7.2. Filtrar palabras vacías (stopwords)

Las palabras más frecuentes suelen ser artículos y preposiciones. Para filtrarlas:

1. **Ve a Settings → Tool Preferences → Word List**

2. **Marca la opción "Use a stoplist below"**

3. **Dos opciones:**

   **Opción A: Usar lista interna**
   - Haz clic en "Add Words"
   - Escribe palabras separadas por Enter:
     ```
     de
     la
     el
     en
     y
     que
     a
     los
     se
     ```
   - Haz clic en "Apply"

   **Opción B: Usar archivo de stopwords**
   - Haz clic en "Open"
   - Selecciona el archivo `stopwords-espanol.txt` (del tutorial de Voyant)
   - Haz clic en "Abrir"

4. **Vuelve a la pestaña "Word List"**

5. **Haz clic en "Start" de nuevo**

6. **Ahora verás palabras de contenido:**
   ```
   Rank  Freq   Word
   1     234    música
   2     198    concierto
   3     156    piano
   4     134    compositor
   5     112    orquesta
   ```

---

### 7.3. Ordenar y filtrar resultados

**Ordenar por:**
- **Rank:** Haz clic en "Rank" (orden por frecuencia)
- **Word:** Haz clic en "Word" (orden alfabético)
- **Freq:** Haz clic en "Freq" (orden por frecuencia)

**Buscar palabra específica:**
- Haz clic derecho en la lista
- Selecciona "Search Term in List"
- Escribe la palabra que buscas

---

### 7.4. Guardar lista de palabras

1. **Ve a File → Save Output to Text File...**
2. **Elige nombre y ubicación:**
   - Ejemplo: `frecuencias_corpus_musical.txt`
3. **Haz clic en "Guardar"**
4. **Abre el archivo con Excel o Notepad**

---

## PASO 8: Concordancias KWIC

### 8.1. ¿Qué son las concordancias?

Las **concordancias** muestran cada aparición de una palabra en su contexto. Es la función más potente de AntConc.

**Ejemplo de concordancia para "piano":**
```
...el concierto de    piano    fue interpretado...
...estudió técnica de piano    en el conservatorio...
...acompañamiento de  piano    y violín sonó...
```

---

### 8.2. Buscar una palabra

1. **Haz clic en la pestaña "Concordance"**

2. **Escribe una palabra en el cuadro "Search Term":**
   - Ejemplo: `piano`

3. **Haz clic en "Start"**

4. **Verás todas las apariciones:**
   - Cada línea muestra la palabra en contexto
   - La palabra buscada está **resaltada en azul** en el centro
   - Texto antes y después de la palabra

**Ejemplo:**
```
File: revista_1920.txt
...la interpretación del     piano     estuvo a cargo...

File: revista_1925.txt
...nuevo método para tocar   piano     fue presentado...

File: revista_1930.txt
...concierto para            piano     y orquesta...
```

---

### 8.3. Opciones de búsqueda avanzada

**Búsqueda simple:**
- `piano` - Busca exactamente "piano"

**Búsqueda con comodines:**
- `piano*` - Busca piano, pianos, pianola, pianista
- `*ista` - Busca pianista, violinista, guitarrista
- `comp?sitor` - Busca compositor o composidor

**Búsqueda de frase:**
- `"música clásica"` - Busca la frase exacta

**Búsqueda por patrón:**
- Marca "Regex" (expresiones regulares)
- `piano|guitarra` - Busca "piano" O "guitarra"
- `(piano|guitarra) (solo|solista)` - Patrones complejos

---

### 8.4. Opciones de visualización

**Cambiar cantidad de contexto:**
1. Ve a **Global Settings → Concordance**
2. **Search Window Size:** Cambia el número (default: 50 caracteres)
   - Más grande = más contexto
   - Más pequeño = más líneas en pantalla

**Ordenar concordancias:**
- Haz clic derecho en el área de resultados
- Selecciona "Sort"
- Opciones:
  - **Sort by 1st Word Right** - Ordena por palabra después
  - **Sort by 1st Word Left** - Ordena por palabra antes
  - **Sort by File Name** - Ordena por archivo

---

### 8.5. Ver contexto completo

1. **Haz clic en cualquier línea de concordancia**

2. **Haz clic en la pestaña "File View"**

3. **Verás el documento completo:**
   - La palabra buscada está resaltada
   - Puedes leer todo el contexto
   - Nombre del archivo arriba

---

### 8.6. Exportar concordancias

1. **Después de buscar una palabra:**
   - File → Save Output to Text File...
   - Elige nombre: `concordancias_piano.txt`
   - Guarda

2. **Abre con Excel o Notepad**

---

## PASO 9: Clusters y N-Grams

### 9.1. ¿Qué son los clusters?

Los **clusters** (o n-grams) son grupos de palabras que aparecen frecuentemente juntas.

**Ejemplos:**
- "música clásica" (bigram = 2 palabras)
- "en el teatro" (trigram = 3 palabras)
- "director de orquesta sinfónica" (4-gram = 4 palabras)

---

### 9.2. Encontrar clusters

1. **Haz clic en la pestaña "Clusters/N-Grams"**

2. **Busca una palabra base:**
   - Escribe en "Search Term": `música`
   - Haz clic en "Start"

3. **Verás clusters que contienen "música":**
   ```
   Freq  Cluster
   45    música clásica
   23    música popular
   18    música española
   12    música contemporánea
   ```

---

### 9.3. Ajustar tamaño de clusters

1. **Ve a "Cluster Size"** (abajo a la izquierda)

2. **Ajusta Min y Max:**
   - **Min: 2, Max: 2** - Solo bigramas (2 palabras)
   - **Min: 3, Max: 3** - Solo trigramas (3 palabras)
   - **Min: 2, Max: 5** - De 2 a 5 palabras

3. **Haz clic en "Start" de nuevo**

---

### 9.4. N-Grams sin palabra base

Para ver TODOS los clusters más frecuentes del corpus:

1. **Borra el "Search Term"** (déjalo vacío)

2. **Configura Cluster Size:**
   - Min: 2, Max: 3

3. **Haz clic en "Start"**

4. **Verás los clusters más frecuentes del corpus completo:**
   ```
   Freq  Cluster
   234   de la música
   189   en el teatro
   156   la ópera italiana
   134   director de orquesta
   ```

---

## PASO 10: Colocaciones (Collocates)

### 10.1. ¿Qué son las colocaciones?

Las **colocaciones** son palabras que aparecen frecuentemente CERCA de otra palabra (pero no necesariamente juntas).

**Ejemplo:** Palabras que aparecen cerca de "piano":
- concierto, solo, teclas, compositor, interpretación

---

### 10.2. Buscar colocaciones

1. **Haz clic en la pestaña "Collocates"**

2. **Escribe una palabra en "Search Term":**
   - Ejemplo: `piano`

3. **Configura ventana de búsqueda:**
   - **Window Span:** 5L to 5R (5 palabras a la izquierda y derecha)

4. **Haz clic en "Start"**

5. **Verás tabla con palabras relacionadas:**
   ```
   Rank  Freq  Stat  Collocate
   1     45    8.3   concierto
   2     34    7.8   solo
   3     28    6.9   compositor
   4     23    6.2   interpretación
   ```

---

### 10.3. Interpretación de resultados

**Columnas:**
- **Freq** - Veces que aparece cerca de tu palabra
- **Stat** - Fuerza de asociación (más alto = más relacionado)
- **Collocate** - La palabra relacionada

**Opciones de estadística:**
- Haz clic en "Stat" para cambiar medida estadística
- **MI (Mutual Information)** - Recomendado
- **T-Score** - Alternativa
- **Log-Likelihood** - Otra opción

---

## PASO 11: Concordance Plot (visualización)

### 11.1. ¿Qué es Concordance Plot?

Es una **visualización gráfica** que muestra DÓNDE aparece una palabra a lo largo de cada documento.

---

### 11.2. Generar visualización

1. **Haz clic en la pestaña "Concordance Plot"**

2. **Escribe palabra en "Search Term":**
   - Ejemplo: `jazz`

3. **Haz clic en "Start"**

4. **Verás gráfico:**
   - Cada archivo es una línea horizontal
   - Marcas verticales = apariciones de la palabra
   - Más marcas = más menciones

**Ejemplo visual:**
```
revista_1920.txt  |      |    |         |
revista_1930.txt  ||   |||  |  ||   ||||   |
revista_1940.txt  ||||||||||||||||||||||||||||
```

En este ejemplo, "jazz" aparece poco en 1920, más en 1930, y mucho en 1940.

---

### 11.3. Comparar dos palabras

1. **Busca primera palabra:** `ópera`
2. **Observa el patrón**
3. **Busca segunda palabra:** `jazz`
4. **Compara los patrones**

**Útil para:**
- Ver evolución de términos en corpus cronológico
- Identificar documentos con mucha/poca mención
- Encontrar patrones de distribución

---

## PASO 12: Keyword List (palabras clave comparativas)

### 12.1. ¿Qué son las keywords?

Las **keywords** son palabras que aparecen **significativamente más** en tu corpus que en un corpus de referencia.

**Ejemplo:**
- Tu corpus: revistas de música clásica
- Corpus de referencia: periódico general
- Keywords: "sinfonía", "orquesta", "director", "partitura" (palabras típicas de música)

---

### 12.2. Crear corpus de referencia

Para usar Keywords necesitas **dos corpus:**

1. **Tu corpus de estudio** (ya cargado)
2. **Un corpus de referencia** (para comparar)

**Opción 1: Usar corpus general del español**
- Descarga corpus de referencia de: http://corpus.rae.es/lfrecuencias.html
- Guarda como archivo .txt

**Opción 2: Crear tu propio corpus de referencia**
- Busca textos generales en español (Wikipedia, periódicos)
- Guárdalos como archivos .txt
- Ponlos en una carpeta separada: `CorpusReferencia`

---

### 12.3. Cargar corpus de referencia

1. **Ve a Settings → Tool Preferences → Keyword List**

2. **Marca "Use raw files"**

3. **Haz clic en "Add Directory"**

4. **Selecciona carpeta de corpus de referencia**

5. **Haz clic en "Load"**

6. **Verás: "Reference Corpus Loaded: X files"**

---

### 12.4. Generar keywords

1. **Haz clic en la pestaña "Keyword List"**

2. **Haz clic en "Start"**

3. **Espera mientras AntConc calcula** (puede tardar 1-2 minutos)

4. **Verás lista de keywords:**
   ```
   Rank  Freq   Keyness  Keyword
   1     456    234.5    sinfonía
   2     389    198.3    orquesta
   3     334    176.8    compositor
   4     298    165.2    director
   ```

**Keyness** = Valor estadístico de lo "característico" que es esa palabra de tu corpus

---

## PASO 13: Configuración y preferencias

### 13.1. Configuración global

**Ve a Global Settings:**
- En Mac: AntConc → Preferences
- En Windows: Settings → Global Settings

**Opciones importantes:**

**Tag Settings:**
- Si tus textos tienen etiquetas XML/HTML, configúralas aquí

**Character Encoding:**
- **Muy importante para español:**
- Selecciona **"UTF-8 (Unicode)"**
- Esto asegura que las tildes (á, é, í) se vean correctamente

**Case:**
- **Treat case as:** Case Insensitive (recomendado para español)
- Esto hace que "Música" = "música" = "MÚSICA"

---

### 13.2. Configuración por herramienta

**Ve a Settings → Tool Preferences:**

Configura cada herramienta individualmente:

**Concordance:**
- Search Window Size: 50-100 (más contexto)
- KWIC Sort: Center

**Word List:**
- Treat all data as lowercase (recomendado)
- Use stoplist (filtrar palabras vacías)

**Clusters:**
- Min cluster size: 2
- Max cluster size: 5
- Min freq: 5 (solo clusters que aparecen 5+ veces)

---

## PASO 14: Casos de uso prácticos

### Ejemplo 1: Análisis de concordancias

**Objetivo:** Estudiar cómo se usa la palabra "mujer" en un corpus

**Pasos:**
1. Carga tu corpus
2. Pestaña "Concordance"
3. Busca: `mujer`
4. Ordena por "1st Word Right" (palabra después)
5. Observa patrones:
   - ¿Con qué adjetivos aparece?
   - ¿En qué contextos se menciona?
6. Exporta resultados

---

### Ejemplo 2: Comparar dos autores

**Objetivo:** Comparar vocabulario de Lorca vs. Machado

**Pasos:**
1. **Primer análisis:**
   - Carga solo archivos de Lorca
   - Genera Word List
   - Guarda como `lorca_frecuencias.txt`

2. **Segundo análisis:**
   - Cierra corpus (File → Close All Files)
   - Carga solo archivos de Machado
   - Genera Word List
   - Guarda como `machado_frecuencias.txt`

3. **Comparación manual:**
   - Abre ambos archivos en Excel
   - Compara las palabras más frecuentes
   - Identifica diferencias de vocabulario

---

### Ejemplo 3: Evolución de términos

**Objetivo:** Ver cómo cambia el uso de "jazz" de 1920 a 1960

**Pasos:**
1. Nombra archivos cronológicamente: `1920_revista.txt`, `1930_revista.txt`, etc.
2. Carga todos en AntConc
3. Pestaña "Concordance Plot"
4. Busca: `jazz`
5. Observa distribución visual:
   - ¿En qué década aparece más?
   - ¿Cuándo empieza a aparecer?
6. Captura pantalla para informe

---

### Ejemplo 4: Buscar expresiones frecuentes

**Objetivo:** Encontrar frases hechas en corpus literario

**Pasos:**
1. Pestaña "Clusters/N-Grams"
2. Deja "Search Term" vacío
3. Cluster Size: Min 3, Max 5
4. Haz clic en "Start"
5. Verás expresiones frecuentes:
   - "en el fondo"
   - "de todos modos"
   - "por otra parte"
6. Exporta lista

---

## PASO 15: Solución de problemas

### Problema 1: Caracteres raros (á = Ã¡)

**Causa:** Archivo no está en UTF-8

**Solución:**
1. Abre el archivo .txt con Notepad (Windows) o TextEdit (Mac)
2. Guarda como → Codificación: UTF-8
3. Vuelve a cargar en AntConc
4. Ve a Global Settings → Character Encoding → UTF-8

---

### Problema 2: No aparecen tildes

**Causa:** Configuración de encoding incorrecta

**Solución:**
1. Global Settings
2. Character Encoding: Selecciona "UTF-8 (Unicode)"
3. Apply
4. Recarga los archivos

---

### Problema 3: AntConc no se abre en Mac

**Causa:** Restricción de seguridad de macOS

**Solución:**
1. Preferencias del Sistema → Seguridad y Privacidad
2. Pestaña General
3. Haz clic en "Abrir de todas formas"
4. Vuelve a intentar abrir AntConc

---

### Problema 4: Word List vacía o con pocas palabras

**Causa:** Stoplist demasiado agresiva

**Solución:**
1. Settings → Tool Preferences → Word List
2. Desmarca "Use a stoplist below"
3. Vuelve a generar Word List

---

### Problema 5: Búsqueda no encuentra nada

**Causa:** Búsqueda case-sensitive o problema de encoding

**Solución:**
1. Global Settings → Case → Case Insensitive
2. Verifica que la palabra esté bien escrita
3. Intenta con comodín: `música*`

---

## PASO 16: Comparación con otras herramientas

| Característica | AntConc | Voyant Tools | Distant Reader |
|----------------|---------|--------------|----------------|
| **Instalación** | Descarga 1 archivo | Ninguna (web) | Compleja (conda) |
| **Dificultad** | ⭐⭐ Media | ⭐ Fácil | ⭐⭐⭐⭐⭐ Muy difícil |
| **Concordancias** | ⭐⭐⭐⭐⭐ Excelente | ⭐⭐⭐ Bueno | ⭐⭐⭐ Bueno |
| **Visualizaciones** | ⭐⭐ Básicas | ⭐⭐⭐⭐⭐ Excelente | ⭐⭐ Básicas |
| **Velocidad** | ⭐⭐⭐⭐⭐ Muy rápido | ⭐⭐⭐ Media | ⭐⭐⭐⭐ Rápido |
| **Offline** | ✅ Sí | ❌ No | ✅ Sí |
| **Corpus grandes** | ✅ Excelente | ⚠️ Limitado | ✅ Bueno |
| **Curva aprendizaje** | 1-2 horas | 15-30 min | 5-10 horas |

---

## PASO 17: Recursos adicionales

### Documentación oficial
- **Página oficial:** https://www.laurenceanthony.net/software/antconc/
- **Help interno:** En AntConc, ve a Help → Help

### Tutoriales en video
- **YouTube:** Busca "AntConc tutorial español"
- **Tutorial oficial (inglés):** https://www.youtube.com/watch?v=3SZlMq8TQIE

### Manuales y guías
- **Programming Historian:** https://programminghistorian.org/es/lecciones/analisis-voyant-tools (incluye sección de AntConc)
- **Corpus linguistics:** https://www.corpuslingua.org/tutorials/antconc/

---

## PASO 18: Ejercicio práctico

### Ejercicio completo (30 minutos)

**Objetivo:** Analizar corpus de 3-5 textos literarios

**Materiales:**
- 3-5 cuentos de un mismo autor en formato .txt
- AntConc instalado

**Actividad:**

1. **[5 min] Preparación:**
   - Descarga 3 cuentos de Borges, Cortázar o García Márquez
   - Guárdalos en carpeta `MiCorpus`
   - Verifica que sean UTF-8

2. **[5 min] Word List:**
   - Carga archivos en AntConc
   - Genera Word List
   - Identifica las 20 palabras más frecuentes
   - Aplica stoplist en español
   - Exporta lista limpia

3. **[10 min] Concordancias:**
   - Busca una palabra temática (ej: "tiempo", "muerte", "casa")
   - Observa contextos
   - Ordena por palabra siguiente
   - Identifica patrones de uso

4. **[5 min] Clusters:**
   - Genera clusters de 2-3 palabras
   - Identifica expresiones frecuentes
   - Exporta lista

5. **[5 min] Concordance Plot:**
   - Visualiza distribución de palabra clave
   - ¿En qué texto aparece más?
   - Captura pantalla

6. **[5 min] Reflexión:**
   - Escribe 1 párrafo sobre:
     * ¿Qué palabras definen al autor?
     * ¿Qué patrones encontraste?
     * ¿Qué te sorprendió?

---

## PASO 19: Consejos finales

### ✅ Mejores prácticas

1. **Corpus limpio:**
   - Elimina encabezados, pies de página
   - Consistente en formato
   - UTF-8 siempre

2. **Nombres de archivo descriptivos:**
   - Incluye fecha, autor, título
   - Ejemplo: `1920_lorca_romancero.txt`

3. **Empieza simple:**
   - Primero Word List
   - Luego Concordance
   - Después funciones avanzadas

4. **Guarda resultados frecuentemente:**
   - Exporta listas importantes
   - No hay "guardar proyecto" en AntConc

5. **Compara corpus:**
   - Analiza un corpus
   - Guarda resultados
   - Analiza otro corpus
   - Compara manualmente

---

### ❌ Errores comunes que evitar

1. **No usar UTF-8:** Caracteres raros
2. **Mezclar idiomas:** Resultados confusos
3. **Nombres de archivo poco claros:** Difícil interpretar Concordance Plot
4. **No filtrar stopwords:** Word List dominada por artículos
5. **Buscar sin comodines:** Te pierdes variaciones (piano/pianos/pianista)

---

## Conclusión

**AntConc es ideal para:**
- ✅ Análisis de concordancias detallado
- ✅ Trabajar offline
- ✅ Corpus grandes (1000+ archivos)
- ✅ Usuarios con algo de experiencia técnica
- ✅ Investigación lingüística seria

**Usa AntConc si:**
- Necesitas concordancias potentes
- Trabajas sin Internet
- Tienes tiempo para aprender (1-2 horas)
- Prefieres software local vs. web

**Usa Voyant Tools si:**
- Necesitas resultados inmediatos
- Prefieres visualizaciones bonitas
- Enseñas a principiantes
- Quieres cero instalación

---

**Tiempo total de aprendizaje:** 1-2 horas para dominar funciones básicas

**¡Empieza ahora descargando:** https://www.laurenceanthony.net/software/antconc/

---

**Última actualización:** Octubre 2025
**Versión de AntConc:** 4.3.1
**Tutorial:** Para estudiantes del Máster en Música Hispana de la Universidad de Salamanca
