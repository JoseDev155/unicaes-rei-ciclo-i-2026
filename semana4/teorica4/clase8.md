# Teórica 4 (REI) - 12/2/2026

* Presentación **Semana 3**: [T3-Tipos de Antenas en Redes con Estandares IEEE-802.11](../../semana3/teorica3/T3-Tipos%20de%20Antenas%20en%20Redes%20con%20Estandares%20IEEE-802.11.pdf)

## **Tema: Tipos de Antenas en Redes**
### ¿Qué es una Antena?
#### Definición básica

* Dispositivo diseñado para **emitir o recibir ondas electromagnéticas**.
* Funciona como **transductor**, convirtiendo *energía eléctrica* en *ondas electromagnéticas*.
* Es un componente esencial en la **comunicación inalámbrica**.

#### Funcionamiento

* Basado en el **principio de reciprocidad electromagnética**.
* Una antena puede:
  * **transmitir señales**
  * **recibir señales**
* En transmisión:
  * *corrientes eléctricas* en *ondas electromagnéticas*.
* En recepción:
  * *ondas electromagnéticas* en *señales eléctricas*.

### Características de las Antenas
#### Ganancia

* Medida de la capacidad de la antena para **concentrar energía en una dirección**.
* Mayor ganancia, **mayor alcance de señal**.

#### Directividad

* Capacidad de **enfocar la energía en una dirección específica**.
* Importante en **comunicaciones punto a punto** de larga distancia.

#### Patrón de Radiación

* Representación de cómo la antena **distribuye energía en el espacio**.
* Tipos:
  * **Omnidireccional**
  * **Direccional**

#### Ancho de Banda

* Rango de **frecuencias en el que la antena opera eficientemente**.
* Mayor ancho de banda, posibilidad de **transmitir más información**.

### Clasificación de las Antenas
#### 1. Por Patrón de Radiación

* Omnidireccionales
* Direccionales
* Sectoriales

#### 2. Por Forma y Construcción

* Dipolo
* Yagi
* Parabólicas
* Panel
* Ranura

#### 3. Por Frecuencia de Operación

* VHF
* UHF
* Microondas
* Milimétricas

#### 4. Por Aplicación

* WiFi
* Celular
* Satelital
* Radio
* TV

### Antenas Omnidireccionales
#### Características

* Emiten señal en **360° en el plano horizontal**.
* Proporcionan **cobertura circular**.

#### Uso en WiFi

* Routers domésticos.
* Puntos de acceso inalámbricos.

#### Aplicación en redes celulares

* Estaciones base de telefonía móvil.

---

Sin embargo, tienen **menor alcance** comparado con antenas direccionales.

### Antenas Direccionales

1. **Enfoque de señal**
   * Concentran energía en **una dirección específica**.
2. **Mayor ganancia**
   * Permiten **mayor alcance y mejor calidad de señal**.
3. **Reducción de interferencias**
   * Reciben señal principalmente de **una dirección**.

Son esenciales en **comunicaciones punto a punto de larga distancia**, como enlaces entre edificios o comunicaciones satelitales.

### Antenas Sectoriales

1. Cobertura en **un sector específico** (60° a 120°).
2. Balance entre antenas:
   * omnidireccionales
   * direccionales.
3. Permiten **diseñar cobertura personalizada**.
4. Mejor **eficiencia energética**.

Uso común:

* **Redes celulares**
* sistemas inalámbricos de gran cobertura

### Antenas de Panel
#### Diseño Compacto

* Estructura **plana y delgada**.
* Instalación discreta en edificios.

#### Directividad Moderada

* Patrón direccional con **haz relativamente amplio**.

#### Versatilidad

* Utilizadas en:
  * redes WiFi
  * telefonía móvil

#### Fácil Integración

* Compatibles con **sistemas MIMO**.

### Antenas Yagi-Uda

Características:

1. Compuesta por:
   * **dipolo activo**
   * elementos pasivos (directores y reflectores).
2. **Alta directividad**
3. **Ganancia ajustable**
   * aumentando el número de directores.
4. **Aplicaciones Variadas**:
   * televisión
   * radio FM
   * radioaficionados
   * enlaces inalámbricos de larga distancia

### Antenas de Parche

También conocidas como **antenas microstrip**.

#### Diseño Plano

* Parche metálico sobre **sustrato dieléctrico**.
* Tamaño compacto.

#### Versatilidad

* Operan en frecuencias desde **MHz hasta GHz**.

#### Patrón de Radiación

* Generalmente **hemisférico**.

### Antenas de Ranura
#### Diseño Único

* Ranura cortada en **superficie conductora**.

#### Aplicaciones Especializadas

* radar
* comunicaciones satelitales
* equipos de medición de alta frecuencia

#### Patrón de Radiación

* **Bidireccional**.

Son apreciadas por su buena **resistencia ambiental**.

### Antenas de Hilo

Tipos principales:

#### 1. Dipolo simple

* Dos conductores en línea recta.
* Patrón de radiación **omnidireccional**.

#### 2. Monopolo

* Mitad de un dipolo.
* Utiliza **plano de tierra**.
* Aplicación:
  * radio AM
  * comunicaciones móviles

#### 3. Antena helicoidal

* Conductor en forma de **hélice**.
* Polarización **circular**.
* Aplicación:
  * comunicaciones satelitales

#### 4. Antena loop

* Conductor formando **bucle cerrado**.
* Usada en **recepción de radio**.

### Antenas de Bocina

1. Apertura en forma de **cuerno o embudo**.
2. **Alta directividad**.
3. Alta eficiencia en **microondas y ondas milimétricas**.
4. Aplicaciones:
   * radioastronomía
   * radar
   * comunicaciones satelitales

### Antenas de Reflector Parabólico
#### Diseño Reflector

* Reflector parabólico que **concentra la señal en el foco**.

#### Alta Ganancia

* Permite **comunicaciones de muy larga distancia**.

#### Aplicaciones

* comunicaciones satelitales
* radiotelescopios
* sistemas de radar

### Antenas de Array

1. Compuestas por **múltiples elementos radiantes**.
2. Control electrónico del **patrón de radiación**.
3. **Direccionamiento adaptativo del haz**.
4. **Alta ganancia** por combinación de señales.
5. Aplicaciones:
   * radar
   * redes **5G**
   * comunicaciones avanzadas

### Ventajas y Desventajas de los Diferentes Tipos de Antenas

| Tipo de Antena    | Ventajas                            | Desventajas         |
|-------------------|-------------------------------------|---------------------|
| Omnidireccionales | Cobertura 360°, instalación simple  | Alcance limitado    |
| Direccionales     | Mayor alcance, menos interferencias | Cobertura limitada  |
| Yagi-Uda          | Alta directividad                   | Banda estrecha      |
| Parabólicas       | Muy alta ganancia                   | Tamaño grande       |
| Array             | Alta ganancia y adaptabilidad       | Complejidad y costo |

### Aplicaciones de los Distintos Tipos de Antenas
#### WiFi y redes locales

* Omnidireccionales
* Panel
* Direccionales para enlaces entre edificios

#### Comunicaciones Satelitales

* Parabólicas
* Helicoidales

#### Redes Celulares

* Sectoriales
* Arrays
* Antenas de parche en dispositivos móviles

#### Sistemas de Radar

* Antenas **array**
* antenas **parabólicas**

### Factores a Considerar al Elegir una Antena

1. **Frecuencia de operación**
2. **Patrón de radiación necesario**
3. **Ganancia y alcance**
4. **Entorno de instalación**
5. **Regulaciones y normativas**

### Instalación y Configuración de Antenas
#### Ubicación Estratégica

* Ubicar en **puntos altos y sin obstáculos**.
* Mantener **línea de vista**.

#### Orientación Precisa

* Alineación correcta en **antenas direccionales**.

#### Cableado Adecuado

* Uso de **cable coaxial de calidad**.
* Reducir longitud para minimizar pérdidas.

#### Protección contra Elementos

* Protección contra **rayos y sobretensiones**.
* Instalación resistente a **condiciones climáticas**.

### Mantenimiento y Cuidado de las Antenas

1. **Inspección regular**
   * detectar daños o desalineación.
2. **Limpieza**
   * eliminar polvo y residuos.
3. **Verificación de conexiones**
   * revisar conectores y corrosión.
4. **Medición de rendimiento**
   * uso de analizadores de espectro.
5. **Actualización o reemplazo**
   * sustituir antenas obsoletas o dañadas.