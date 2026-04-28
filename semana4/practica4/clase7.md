# Práctica 4 (REI) - 11/2/2026
## Descripción de la práctica

Recorrer los edificios "F", "E" y "D" (oficinas administrativas de Registro Académico) y obtener las siguientes mediciones:

* Intensidad de la señal
* Identificar redes
* Identificar los SSIDs
* Identificar los Proveedores de Internet

* Documento de apoyo: `Actividad Redes Inalambricas ISP-Desde Casa.docx`

>Me tocó el Edificio "D"

## Resultados - Edificio "D"

* Aplicación utilizada: **Opensignal**

### Parte 1: Identificación de dispositivos
#### Nombre del ISP
##### Proveedores encontrados

* Proveedor de UNICAES: **Claro**

| Operador | Bajada (Mbps)  | Subida (Mbps) | Latencia (ms) | Señal (hasta 5 barras) |
|----------|----------------|---------------|---------------|------------------------|
| Claro    | 22.74          | 9.98          | 67            | 4/5                    |
| Movistar | 9.56           | 5.79          | 232           | 3/5                    |
| Tigo     | 10.36          | 5.46          | 107           | 4/5                    |

#### Marca y modelo

* Marca: **Access Point Cisco**
* Modelo: *Desconocido*

>Dispositivos no visibles, pero se asume que están dentro de las instalaciones del Edificio "D".

#### Función del dispositivo o dispositivos

Un Access Point (AP) actúa como un puente entre la red cableada y los dispositivos inalámbricos, permitiendo ampliar la cobertura Wi-Fi y mejorar la conectividad de la red.

### Parte 2: Análisis de la red inalámbrica

* Nombre de la red Wi-Fi: `Catolica_WiFi_GHI` (red predominante)
>También se detectaron las redes: `B`, `F`, pero su señal es débil en algunos puntos

* Calidad de la señal: **3/5 en promedio (Buena)**

Datos de:
* SSID
* Tipo de seguridad
* Banda utilizada (2.4 GHz / 5 GHz / 6GHz)
* Cantidad de dispositivos conectados

No pueden ser recopilados con **Opensignal**.

### Parte 3: Prueba de conexión

**Consideraciones:** Los resultados están sujetos a las condiciones climáticas que azotan al país y la hora en que fueron hechas:

* Condiciones climáticas: Fuertes vientos
* Hora: Noche, de 6:35 - 8:20 p.m.
* Instalaciones interiores y 2da planta cerradas por la hora, por lo que no se pudo hacer mediciones en esas zonas

#### Tabla de mediciones

<table>
  <thead>
    <tr>
      <th rowspan="2">Edificio</th>
      <th rowspan="2">Planta</th>
      <th rowspan="2">Zona</th>
      <th rowspan="2">Distancia desde la zona anterior (m)</th>
      <th rowspan="2">SSID</th>
      <th colspan="3">Conectividad</th>
    </tr>
    <tr>
      <th>Bajada/Descarga (Mbps)</th>
      <th>Subida (Mbps)</th>
      <th>Latencia (ms)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="6">D</td>
      <td rowspan="3">Baja - INTERIOR</td>
      <td>Ventanilla de <em>Contabilidad</em>, lado DERECHO</td>
      <td>0</td>
      <td>x</td>
      <td>13.3</td>
      <td>7.79</td>
      <td>2328</td>
    </tr>
    <tr>
      <td>Ventanilla de <em>Registro Académico</em>, lado IZQUIERDO</td>
      <td>4</td>
      <td>x</td>
      <td>14.1</td>
      <td>11.6</td>
      <td>38</td>
    </tr>
    <tr>
      <td>Entrada corporativa, <em>Registro Académico</em>, lado IZQUIERDO</td>
      <td>4</td>
      <td>x</td>
      <td>7.96</td>
      <td>5.74</td>
      <td>36</td>
    </tr>
    <tr>
      <td rowspan="3">Baja - EXTERIOR</td>
      <td>Mitad de gradas, lado DERECHO</td>
      <td>12</td>
      <td>x</td>
      <td>14.9</td>
      <td>11.5</td>
      <td>37</td>
    </tr>
    <tr>
      <td>Mitad de gradas, lado IZQUIERDO</td>
      <td>7</td>
      <td>x</td>
      <td>14.9</td>
      <td>13.3</td>
      <td>42</td>
    </tr>
    <tr>
      <td>Mitad de parqueo, centro del edificio</td>
      <td>10</td>
      <td>x</td>
      <td>14.3</td>
      <td>14.4</td>
      <td>37</td>
    </tr>
  </tbody>
</table>

### Parte 4: Reflexión y mejoras
#### ¿El servicio cumple con las necesidades del hogar? (edificio)

El servicio de conectividad en el **Edificio "D"** presenta características mixtas. Claro ofrece velocidades de bajada adecuadas (22.74 Mbps)
con buena latencia (67 ms), lo que es suficiente para operaciones administrativas básicas. Sin embargo, la red Wi-Fi presenta latencias
extremadamente altas en algunas zonas interiores (2328 ms en la ventanilla de Contabilidad), lo que afecta significativamente la
experiencia del usuario. En general, el servicio cubre las necesidades básicas administrativas, pero con limitaciones importantes en ciertas ubicaciones.

#### Problemas detectados

* **Latencia crítica**: Picos de latencia extremadamente altos (2328 ms) en zonas interiores, particularmente en la ventanilla de Contabilidad.
* **Inconsistencia de señal**: Variación significativa en la calidad de conexión entre diferentes puntos del edificio.
* **Cobertura desigual**: Aunque se detecta señal en todo el edificio, la calidad fluctúa entre interior y exterior (3/5 en promedio).
* **Interferencia en zonas interiores**: Las zonas interiores muestran mayor latencia que las exteriores, lo que sugiere problemas de penetración de señal o interferencia.

#### Propuestas de mejora

* **Reubicación o adición de Access Points**: Aumentar el número de APs o reposicionarlos para mejorar la cobertura en zonas interiores, especialmente cerca de las áreas administrativas.
* **Cambio de canal Wi-Fi**: Realizar un análisis de interferencia (con **NetSpot**, por ejemplo) y cambiar a un canal Wi-Fi menos congestionado para optimizar el rendimiento.
* **Mantenimiento preventivo**: Realizar limpieza y revisión de los dispositivos Cisco para asegurar un óptimo funcionamiento.

---

* Documento final: `Practica4-ActividadRedes.pdf`