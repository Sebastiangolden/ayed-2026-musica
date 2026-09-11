# Informe del TP

Completar y hacer crecer en cada entrega. No hace falta prosa larga: oraciones claras y tablas.

## 1. Grupo y tema

- Tema: Biblioteca musical
- Nuestra motivación: Elegimos trabajar con una biblioteca musical porque nos resulta un dominio cercano y fácil de entender: todos tenemos experiencia con canciones, artistas y álbumes, lo que hace más intuitivo pensar en cómo representarlos en código. Además, este tema nos permite mostrar con claridad la diferencia entre datos que deben preservarse y datos que pueden cambiar. Por ejemplo, el título original de una canción o el año de publicación son información histórica que no tendría sentido modificar, mientras que el catálogo como conjunto sí puede crecer o actualizarse con nuevas canciones. En ese sentido, la música nos da un contexto atractivo y, al mismo tiempo, útil para justificar decisiones de diseño en estructuras de datos.

## 2. Modelo

En nuestro modelo, un ítem del catálogo es una canción. Cada canción tiene los siguientes atributos:
id: identificador único
titulo: nombre de la canción
artista: intérprete principal
album: disco al que pertenece
genero: estilo musical
anio: año de publicación
duracion_seg: duración en segundos

Mutables: usamos listas y diccionarios para representar el catálogo y las canciones. La lista es mutable porque necesitamos poder agregar o quitar canciones, y el diccionario es mutable porque puede ser necesario corregir o completar atributos (por ejemplo, si faltaba el género o se escribió mal la duración). Esta flexibilidad es importante para que el sistema evolucione.

Inmutables: los atributos básicos de cada canción (título, artista, álbum, género, año, duración) se manejan como strings o enteros, que son inmutables en Python. La decisión de mantenerlos así busca evitar efectos secundarios: si alguien consulta el catálogo, debe confiar en que el título “Algo contigo” siempre será ese y no se va a modificar accidentalmente. Esto protege la integridad de los datos históricos y asegura consistencia en las búsquedas.

## 3. Recursión (E2)

- Función:
- Caso base:
- Caso recursivo:
- Traza de un ejemplo real del dataset:

## 4. TADs (E3)

| TAD | Operaciones | Invariante |
| --- | --- | --- |
| ListaEnlazada |  |  |
| Pila |  |  |
| Cola |  |  |

Dónde se usa cada uno en el dominio.

## 5. Complejidad (E4)

| Operación | Tiempo | Espacio | Por qué |
| --- | --- | --- | --- |
|  |  |  |  |

Mediciones (`time.perf_counter`):

| Operación | n | segundos |
| --- | --- | --- |
|  |  |  |

## 6. Persistencia (E5)

- Layout del registro binario (campos, `struct`, anchos):
- Header:
- Cómo se actualiza un registro por posición:

## 7. Reparto de trabajo (E6)

| Integrante | Qué hizo | Qué puede defender |
| --- | --- | --- |
|  |  |  |
