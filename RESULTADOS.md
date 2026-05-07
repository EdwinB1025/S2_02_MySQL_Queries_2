# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 7 correctas de 23 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.45 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
 id | nombre | apellido1 | apellido2 | fecha_nacimiento
+22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
 7.00 | Ismael | Strosin | Turcotte | 1999-05-24
-22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
```

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 6: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
-apellido1 | apellido2 | nombre | departamento
-Fahey | Considine | Antonio | Economía y Empresa
+apellido1 | apellido2 | nombre | nombre
+Ramirez | Gea | Zoe | Informática
+Schmidt | Fisher | David | Matemáticas
+Lemke | Rutherford | Cristina | Economía y Empresa
+Spencer | Lakin | Esther | Educación
+Streich | Hirthe | Carmen | Educación
+Stiedemann | Morissette | Alfredo | Química y Física
 Hamill | Kozey | Manolo | Informática
 Kohler | Schoen | Alejandro | Matemáticas
-Lemke | Rutherford | Cristina | Economía y Empresa
+Fahey | Considine | Antonio | Economía y Empresa
+Ruecker | Upton | Guillermo | Educación
 Monahan | Murray | Micaela | Agronomía
-Ramirez | Gea | Zoe | Informática
-Ruecker | Upton | Guillermo | Educación
-Schmidt | Fisher | David | Matemáticas
 Schowalter | Muller | Francesca | Química y Física
-Spencer | Lakin | Esther | Educación
-Stiedemann | Morissette | Alfredo | Química y Física
-Streich | Hirthe | Carmen | Educación
```

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.47 ms
✅ Se usó índice(s) en la consulta: nif, PRIMARY

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, id_profesor,id_grado, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ❌ Query 10: Error
- **Descripción**: 'NoneType' object is not iterable


## ❌ Query 11: Incorrecto
```diff
--- 
+++ 
@@ -1 +1,14 @@
-apellido1 | apellido2 | nombre
+nombre_departamento | apellido1 | apellido2 | nombre
+NULL | Barrera | Ceron | Edwin
+Agronomía | Monahan | Murray | Micaela
+Economía y Empresa | Fahey | Considine | Antonio
+Economía y Empresa | Lemke | Rutherford | Cristina
+Educación | Ruecker | Upton | Guillermo
+Educación | Spencer | Lakin | Esther
+Educación | Streich | Hirthe | Carmen
+Informática | Hamill | Kozey | Manolo
+Informática | Ramirez | Gea | Zoe
+Matemáticas | Kohler | Schoen | Alejandro
+Matemáticas | Schmidt | Fisher | David
+Química y Física | Schowalter | Muller | Francesca
+Química y Física | Stiedemann | Morissette | Alfredo
```

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 12: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,2 @@
-nombre
-Filología
-Derecho
-Biología y Geología
+apellido1 | apellido2 | nombre
+Barrera | Ceron | Edwin
```

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 13: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,4 @@
-apellido1 | apellido2 | nombre
-Schmidt | Fisher | David
-Kohler | Schoen | Alejandro
-Lemke | Rutherford | Cristina
-Fahey | Considine | Antonio
-Spencer | Lakin | Esther
-Streich | Hirthe | Carmen
-Ruecker | Upton | Guillermo
-Monahan | Murray | Micaela
-Stiedemann | Morissette | Alfredo
-Schowalter | Muller | Francesca
+nombre
+Filología
+Derecho
+Biología y Geología
```

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 14: Incorrecto
```diff
--- 
+++ 
@@ -1,63 +1,12 @@
-id | nombre
-22.00 | Ingeniería de Requisitos
-23.00 | Integración de las Tecnologías de la Información en las Organizaciones
-24.00 | Modelado y Diseño del Software 1
-25.00 | Multiprocesadores
-26.00 | Seguridad y cumplimiento normativo
-27.00 | Sistema de Información para las Organizaciones
-28.00 | Tecnologías web
-29.00 | Teoría de códigos y criptografía
-30.00 | Administración de bases de datos
-31.00 | Herramientas y Métodos de Ingeniería del Software
-32.00 | Informática industrial y robótica
-33.00 | Ingeniería de Sistemas de Información
-34.00 | Modelado y Diseño del Software 2
-35.00 | Negocio Electrónico
-36.00 | Periféricos e interfaces
-37.00 | Sistemas de tiempo real
-38.00 | Tecnologías de acceso a red
-39.00 | Tratamiento digital de imágenes
-40.00 | Administración de redes y sistemas operativos
-41.00 | Almacenes de Datos
-42.00 | Fiabilidad y Gestión de Riesgos
-43.00 | Líneas de Productos Software
-44.00 | Procesos de Ingeniería del Software 1
-45.00 | Tecnologías multimedia
-46.00 | Análisis y planificación de las TI
-47.00 | Desarrollo Rápido de Aplicaciones
-48.00 | Gestión de la Calidad y de la Innovación Tecnológica
-49.00 | Inteligencia del Negocio
-50.00 | Procesos de Ingeniería del Software 2
-51.00 | Seguridad Informática
-52.00 | Biologia celular
-53.00 | Física
-54.00 | Matemáticas I
-55.00 | Química general
-56.00 | Química orgánica
-57.00 | Biología vegetal y animal
-58.00 | Bioquímica
-59.00 | Genética
-60.00 | Matemáticas II
-61.00 | Microbiología
-62.00 | Botánica agrícola
-63.00 | Fisiología vegetal
-64.00 | Genética molecular
-65.00 | Ingeniería bioquímica
-66.00 | Termodinámica y cinética química aplicada
-67.00 | Biorreactores
-68.00 | Biotecnología microbiana
-69.00 | Ingeniería genética
-70.00 | Inmunología
-71.00 | Virología
-72.00 | Bases moleculares del desarrollo vegetal
-73.00 | Fisiología animal
-74.00 | Metabolismo y biosíntesis de biomoléculas
-75.00 | Operaciones de separación
-76.00 | Patología molecular de plantas
-77.00 | Técnicas instrumentales básicas
-78.00 | Bioinformática
-79.00 | Biotecnología de los productos hortofrutículas
-80.00 | Biotecnología vegetal
-81.00 | Genómica y proteómica
-82.00 | Procesos biotecnológicos
-83.00 | Técnicas instrumentales avanzadas
+apellido1 | apellido2 | nombre
+Schmidt | Fisher | David
+Lemke | Rutherford | Cristina
+Spencer | Lakin | Esther
+Streich | Hirthe | Carmen
+Stiedemann | Morissette | Alfredo
+Kohler | Schoen | Alejandro
+Fahey | Considine | Antonio
+Ruecker | Upton | Guillermo
+Monahan | Murray | Micaela
+Schowalter | Muller | Francesca
+Barrera | Ceron | Edwin
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: <auto_distinct_key>, id_profesor

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,63 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
+id | nombre
+22.00 | Ingeniería de Requisitos
+23.00 | Integración de las Tecnologías de la Información en las Organizaciones
+24.00 | Modelado y Diseño del Software 1
+25.00 | Multiprocesadores
+26.00 | Seguridad y cumplimiento normativo
+27.00 | Sistema de Información para las Organizaciones
+28.00 | Tecnologías web
+29.00 | Teoría de códigos y criptografía
+30.00 | Administración de bases de datos
+31.00 | Herramientas y Métodos de Ingeniería del Software
+32.00 | Informática industrial y robótica
+33.00 | Ingeniería de Sistemas de Información
+34.00 | Modelado y Diseño del Software 2
+35.00 | Negocio Electrónico
+36.00 | Periféricos e interfaces
+37.00 | Sistemas de tiempo real
+38.00 | Tecnologías de acceso a red
+39.00 | Tratamiento digital de imágenes
+40.00 | Administración de redes y sistemas operativos
+41.00 | Almacenes de Datos
+42.00 | Fiabilidad y Gestión de Riesgos
+43.00 | Líneas de Productos Software
+44.00 | Procesos de Ingeniería del Software 1
+45.00 | Tecnologías multimedia
+46.00 | Análisis y planificación de las TI
+47.00 | Desarrollo Rápido de Aplicaciones
+48.00 | Gestión de la Calidad y de la Innovación Tecnológica
+49.00 | Inteligencia del Negocio
+50.00 | Procesos de Ingeniería del Software 2
+51.00 | Seguridad Informática
+52.00 | Biologia celular
+53.00 | Física
+54.00 | Matemáticas I
+55.00 | Química general
+56.00 | Química orgánica
+57.00 | Biología vegetal y animal
+58.00 | Bioquímica
+59.00 | Genética
+60.00 | Matemáticas II
+61.00 | Microbiología
+62.00 | Botánica agrícola
+63.00 | Fisiología vegetal
+64.00 | Genética molecular
+65.00 | Ingeniería bioquímica
+66.00 | Termodinámica y cinética química aplicada
+67.00 | Biorreactores
+68.00 | Biotecnología microbiana
+69.00 | Ingeniería genética
+70.00 | Inmunología
+71.00 | Virología
+72.00 | Bases moleculares del desarrollo vegetal
+73.00 | Fisiología animal
+74.00 | Metabolismo y biosíntesis de biomoléculas
+75.00 | Operaciones de separación
+76.00 | Patología molecular de plantas
+77.00 | Técnicas instrumentales básicas
+78.00 | Bioinformática
+79.00 | Biotecnología de los productos hortofrutículas
+80.00 | Biotecnología vegetal
+81.00 | Genómica y proteómica
+82.00 | Procesos biotecnológicos
+83.00 | Técnicas instrumentales avanzadas
```

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,74 @@
-total
-12.00
+nombre
+Arquitectura de Computadores
+Estructura de Datos y Algoritmos I
+Ingeniería del Software
+Sistemas Inteligentes
+Sistemas Operativos
+Bases de Datos
+Estructura de Datos y Algoritmos II
+Fundamentos de Redes de Computadores
+Planificación y Gestión de Proyectos Informáticos
+Programación de Servicios Software
+Desarrollo de interfaces de usuario
+Ingeniería de Requisitos
+Integración de las Tecnologías de la Información en las Organizaciones
+Modelado y Diseño del Software 1
+Multiprocesadores
+Seguridad y cumplimiento normativo
+Sistema de Información para las Organizaciones
+Tecnologías web
+Teoría de códigos y criptografía
+Administración de bases de datos
+Herramientas y Métodos de Ingeniería del Software
+Informática industrial y robótica
+Ingeniería de Sistemas de Información
+Modelado y Diseño del Software 2
+Negocio Electrónico
+Periféricos e interfaces
+Sistemas de tiempo real
+Tecnologías de acceso a red
+Tratamiento digital de imágenes
+Administración de redes y sistemas operativos
+Almacenes de Datos
+Fiabilidad y Gestión de Riesgos
+Líneas de Productos Software
+Procesos de Ingeniería del Software 1
+Tecnologías multimedia
+Análisis y planificación de las TI
+Desarrollo Rápido de Aplicaciones
+Gestión de la Calidad y de la Innovación Tecnológica
+Inteligencia del Negocio
+Procesos de Ingeniería del Software 2
+Seguridad Informática
+Biologia celular
+Física
+Matemáticas I
+Química general
+Química orgánica
+Biología vegetal y animal
+Bioquímica
+Genética
+Matemáticas II
+Microbiología
+Botánica agrícola
+Fisiología vegetal
+Genética molecular
+Ingeniería bioquímica
+Termodinámica y cinética química aplicada
+Biorreactores
+Biotecnología microbiana
+Ingeniería genética
+Inmunología
+Virología
+Bases moleculares del desarrollo vegetal
+Fisiología animal
+Metabolismo y biosíntesis de biomoléculas
+Operaciones de separación
+Patología molecular de plantas
+Técnicas instrumentales básicas
+Bioinformática
+Biotecnología de los productos hortofrutículas
+Biotecnología vegetal
+Genómica y proteómica
+Procesos biotecnológicos
+Técnicas instrumentales avanzadas
```

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: id_asignatura

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
 total
-2.00
+12.00
```

⏱ Tiempo: 0.26 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 18: Incorrecto
```diff
--- 
+++ 
@@ -1,7 +1,2 @@
-departamento | total
-Educación | 3.00
-Informática | 2.00
-Matemáticas | 2.00
-Economía y Empresa | 2.00
-Química y Física | 2.00
-Agronomía | 1.00
+total
+2.00
```

⏱ Tiempo: 0.26 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,7 @@
-departamento | total
+nombre | total
+Agronomía | 1.00
 Informática | 2.00
 Matemáticas | 2.00
 Economía y Empresa | 2.00
+Química y Física | 2.00
 Educación | 3.00
-Agronomía | 1.00
-Química y Física | 2.00
-Filología | 0.00
-Derecho | 0.00
-Biología y Geología | 0.00
```

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,11 +1,10 @@
-grau | total
-Grado en Ingeniería Informática (Plan 2015) | 51.00
-Grado en Biotecnología (Plan 2015) | 32.00
-Grado en Ingeniería Agrícola (Plan 2015) | 0.00
-Grado en Ingeniería Eléctrica (Plan 2014) | 0.00
-Grado en Ingeniería Electrónica Industrial (Plan 2010) | 0.00
-Grado en Ingeniería Mecánica (Plan 2010) | 0.00
-Grado en Ingeniería Química Industrial (Plan 2010) | 0.00
-Grado en Ciencias Ambientales (Plan 2009) | 0.00
-Grado en Matemáticas (Plan 2010) | 0.00
-Grado en Química (Plan 2009) | 0.00
+nombre | total
+Agronomía | 1.00
+Filología | 1.00
+Derecho | 1.00
+Biología y Geología | 1.00
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Química y Física | 2.00
+Educación | 3.00
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, PRIMARY

---

## ❌ Query 21: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,11 @@
-grau | total
+grado | total
+Grado en Ingeniería Agrícola (Plan 2015) | 1.00
+Grado en Ingeniería Eléctrica (Plan 2014) | 1.00
+Grado en Ingeniería Electrónica Industrial (Plan 2010) | 1.00
+Grado en Ingeniería Mecánica (Plan 2010) | 1.00
+Grado en Ingeniería Química Industrial (Plan 2010) | 1.00
+Grado en Ciencias Ambientales (Plan 2009) | 1.00
+Grado en Matemáticas (Plan 2010) | 1.00
+Grado en Química (Plan 2009) | 1.00
+Grado en Biotecnología (Plan 2015) | 32.00
 Grado en Ingeniería Informática (Plan 2015) | 51.00
```

⏱ Tiempo: 0.29 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,6 +1,2 @@
-grau | tipo | total_creditos
-Grado en Ingeniería Informática (Plan 2015) | básica | 72.00
-Grado en Ingeniería Informática (Plan 2015) | obligatoria | 54.00
-Grado en Ingeniería Informática (Plan 2015) | optativa | 180.00
-Grado en Biotecnología (Plan 2015) | básica | 60.00
-Grado en Biotecnología (Plan 2015) | obligatoria | 120.00
+grado | total
+Grado en Ingeniería Informática (Plan 2015) | 51.00
```

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 23: Error
- **Descripción**: 'NoneType' object is not iterable

