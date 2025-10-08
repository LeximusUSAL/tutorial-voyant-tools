# Ejercicios Prácticos con Voyant Tools

## Ejercicio 1: Análisis básico (15 minutos)

### Objetivo
Familiarizarse con la interfaz de Voyant Tools

### Pasos

1. **Preparación:**
   - Ve a https://voyant-tools.org
   - Copia este texto en el cuadro principal:

```
El Quijote es la obra más famosa de Cervantes. Don Quijote y Sancho Panza recorren
La Mancha en busca de aventuras. Don Quijote lucha contra molinos de viento pensando
que son gigantes. Sancho Panza es el fiel escudero de Don Quijote. La obra es una
crítica de las novelas de caballería. Cervantes escribió Don Quijote en el siglo XVII.
```

2. **Análisis:**
   - Haz clic en "Revelar"
   - Observa la nube de palabras
   - **Pregunta 1:** ¿Cuáles son las 3 palabras más frecuentes?
   - **Pregunta 2:** ¿Cuántas veces aparece "Quijote"?

3. **Contextos:**
   - Busca la palabra "Quijote" en el panel Contexts
   - **Pregunta 3:** ¿En qué contextos aparece?

---

## Ejercicio 2: Comparar dos textos (20 minutos)

### Objetivo
Aprender a comparar vocabulario entre documentos

### Materiales necesarios
Crea dos archivos de texto:

**archivo1.txt** (Texto romántico):
```
El amor es eterno. Los corazones enamorados bailan bajo la luna.
Las flores del jardín perfuman la noche romántica. El beso dulce
sella el amor verdadero. La pasión arde como fuego eterno.
```

**archivo2.txt** (Texto científico):
```
El experimento requiere precisión. Los datos científicos confirman
la hipótesis. El laboratorio mantiene temperatura constante. La
metodología experimental garantiza resultados precisos. El análisis
estadístico valida las conclusiones.
```

### Pasos

1. Sube ambos archivos a Voyant Tools
2. Observa las palabras más frecuentes en Cirrus
3. **Pregunta 1:** ¿Qué palabras definen cada texto?
4. Usa el panel Terms para ver frecuencias exactas
5. **Pregunta 2:** ¿Qué palabras son únicas de cada texto?

---

## Ejercicio 3: Análisis de tendencias (25 minutos)

### Objetivo
Usar Trends para ver evolución de términos

### Materiales
Crea 3 archivos cronológicos simulando noticias:

**1900.txt**:
```
El piano es el instrumento rey en los salones aristocráticos.
Las óperas italianas dominan los teatros europeos. El violín
acompaña las veladas musicales de la alta sociedad.
```

**1950.txt**:
```
El jazz revoluciona la música popular. La guitarra eléctrica
transforma el rock and roll. La radio difunde nuevos géneros
musicales a millones de oyentes.
```

**2000.txt**:
```
La música electrónica domina los clubs. Los sintetizadores crean
sonidos digitales. Internet permite descargar canciones. Los DJs
son las nuevas estrellas musicales.
```

### Pasos

1. Sube los 3 archivos a Voyant
2. En el panel Trends, busca: "piano", "guitarra", "electrónica"
3. **Pregunta 1:** ¿Qué palabra desaparece con el tiempo?
4. **Pregunta 2:** ¿Qué palabra aparece solo al final?
5. Exporta el gráfico de tendencias

---

## Ejercicio 4: Concordancias KWIC (20 minutos)

### Objetivo
Analizar palabras en contexto

### Material
Usa este texto:

```
La música clásica requiere formación técnica. El músico de jazz improvisa
constantemente. La música popular conecta con las masas. El músico clásico
interpreta partituras. La música folclórica preserva tradiciones. El músico
de rock experimenta con amplificación. La música contemporánea rompe esquemas.
```

### Pasos

1. Sube el texto a Voyant
2. En Contexts, busca "música"
3. **Pregunta 1:** ¿Con qué adjetivos se asocia "música"?
4. Ahora busca "músico"
5. **Pregunta 2:** ¿Qué acciones realizan los músicos?
6. Exporta las concordancias como CSV

---

## Ejercicio 5: Filtrar stopwords (30 minutos)

### Objetivo
Aprender a personalizar el análisis filtrando palabras

### Material
Texto con muchas palabras repetidas:

```
El señor González, don Manuel, fue un gran pianista. El señor González
tocaba el piano todos los días. Don Manuel estudió en el conservatorio.
El piano del señor González era un Steinway. Don Manuel dio conciertos
por toda España. El señor González falleció en 1950.
```

### Pasos SIN filtrar

1. Sube el texto a Voyant normalmente
2. Observa Cirrus
3. **Pregunta 1:** ¿Qué palabras repetitivas ves?

### Pasos CON filtro

4. Haz clic en "Options" antes de subir
5. En "Stopwords", selecciona "Edit List"
6. Añade estas palabras (una por línea):
```
señor
don
manuel
gonzález
```
7. Sube el texto de nuevo
8. **Pregunta 2:** ¿Cómo cambia la nube de palabras?

---

## Ejercicio 6: Correlaciones (25 minutos)

### Objetivo
Descubrir qué palabras aparecen juntas

### Material
Texto sobre instrumentos musicales:

```
El piano requiere afinación constante. El pianista practica escalas diariamente.
La guitarra española tiene seis cuerdas. El guitarrista flamenco domina el rasgueo.
El violín produce sonido con arco. El violinista debe tener oído absoluto.
La trompeta suena en las orquestas de jazz. El trompetista necesita gran capacidad pulmonar.
```

### Pasos

1. Sube el texto a Voyant
2. Cambia un panel a "Correlations" (usa el icono de ventanas)
3. Selecciona "piano"
4. **Pregunta 1:** ¿Qué palabras correlacionan con "piano"?
5. Ahora selecciona "guitarra"
6. **Pregunta 2:** ¿Son diferentes las correlaciones?
7. **Pregunta 3:** ¿Qué patrón observas?

---

## Ejercicio 7: Proyecto completo (45-60 minutos)

### Objetivo
Realizar un análisis completo de corpus

### Material
Busca en Internet 5-10 cuentos cortos de un mismo autor (por ejemplo, Borges, Cortázar, Poe) en formato .txt

### Pasos

1. **Preparación (10 min):**
   - Descarga 5-10 cuentos del mismo autor
   - Guárdalos como .txt con nombres claros
   - Verifica que estén en UTF-8

2. **Análisis exploratorio (10 min):**
   - Sube todos los archivos a Voyant
   - Observa Cirrus
   - Anota las 20 palabras más frecuentes
   - Ve Summary para estadísticas generales

3. **Análisis de términos clave (10 min):**
   - Identifica 3-5 palabras temáticas importantes
   - Usa Contexts para ver cómo se usan
   - Usa Trends para ver si algunas aparecen más en ciertos cuentos

4. **Correlaciones (10 min):**
   - Busca correlaciones de las palabras clave
   - Identifica patrones temáticos

5. **Exportación (5 min):**
   - Exporta nube de palabras como imagen
   - Exporta tabla de términos como CSV
   - Guarda la URL del análisis

6. **Interpretación (10 min):**
   - Escribe 1 párrafo respondiendo:
     * ¿Qué temas dominan la obra del autor?
     * ¿Qué palabras te sorprendieron?
     * ¿Qué patrones lingüísticos observaste?

---

## Ejercicio 8: Análisis de prensa (30 minutos)

### Objetivo
Simular análisis de noticias históricas

### Material
Crea 3 archivos simulando portadas de periódico:

**1918_gripe.txt**:
```
La gripe española causa miles de víctimas. Los hospitales están saturados.
Las autoridades recomiendan evitar aglomeraciones. La pandemia afecta
gravemente la economía. Los médicos trabajan sin descanso.
```

**1936_guerra.txt**:
```
La guerra civil divide España. Las tropas avanzan hacia Madrid.
Los bombardeos causan destrucción. Los refugiados huyen de las zonas
de combate. La situación es cada vez más grave.
```

**1969_luna.txt**:
```
El hombre llega a la Luna. Armstrong pisa suelo lunar. La NASA celebra
el éxito histórico. La carrera espacial alcanza su momento cumbre.
La tecnología hace posible lo imposible.
```

### Pasos

1. Sube los 3 archivos a Voyant
2. **Pregunta 1:** ¿Qué palabras definen cada época?
3. Usa Trends para comparar: "guerra", "hospital", "tecnología"
4. **Pregunta 2:** ¿Qué tendencias observas?
5. Usa Reader para leer cada texto completo
6. **Pregunta 3:** ¿Cómo cambia el tono entre épocas?

---

## Ejercicio 9: Trabajar con stopwords en español (20 minutos)

### Objetivo
Dominar el filtrado de palabras vacías

### Material
Cualquier texto en español de 200+ palabras

### Pasos

1. **Primera pasada:**
   - Sube texto SIN configurar stopwords
   - Observa qué palabras dominan

2. **Segunda pasada:**
   - Options → Stopwords → Spanish
   - Sube de nuevo
   - **Pregunta 1:** ¿Qué cambió?

3. **Tercera pasada (personalizada):**
   - Edit List → añade palabras específicas que no quieres
   - Ejemplos para textos musicales:
     ```
     señor
     señora
     don
     doña
     ```
   - **Pregunta 2:** ¿Mejoraron los resultados?

---

## Ejercicio 10: Exportar y presentar (30 minutos)

### Objetivo
Crear una presentación con resultados de Voyant

### Pasos

1. **Análisis (15 min):**
   - Elige un corpus de 3-5 textos
   - Realiza análisis completo con Voyant

2. **Exportación (10 min):**
   - Exporta nube de palabras (PNG)
   - Exporta gráfico de tendencias (PNG)
   - Exporta tabla de términos (CSV)
   - Copia la URL del análisis

3. **Presentación (5 min):**
   - Crea un documento/presentación con:
     * Título del corpus
     * Imagen de nube de palabras
     * Tabla de 10 palabras más frecuentes
     * Gráfico de tendencias
     * 1 párrafo de interpretación
     * URL para acceso completo

---

## Recursos para ejercicios

### Textos de dominio público en español
- **Cervantes Virtual:** http://www.cervantesvirtual.com
- **Wikisource español:** https://es.wikisource.org
- **Proyecto Gutenberg (español):** https://www.gutenberg.org/browse/languages/es

### Corpus de ejemplo
- **CORDE:** Corpus diacrónico del español
- **CREA:** Corpus de referencia del español actual
- **Brown Corpus (adaptado):** Corpus balanceado

---

## Evaluación de aprendizaje

Después de completar los ejercicios, deberías poder:

- ✅ Subir textos a Voyant Tools
- ✅ Interpretar nubes de palabras
- ✅ Analizar frecuencias de términos
- ✅ Usar concordancias para análisis cualitativo
- ✅ Comparar textos con Trends
- ✅ Filtrar palabras vacías
- ✅ Exportar visualizaciones y datos
- ✅ Crear presentaciones con resultados

---

**¡Practica estos ejercicios antes de tu clase para estar preparado/a!**
