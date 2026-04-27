# Configuración de un Access Point para Mesh en Exterior

>Resolución de preguntas

## Paso 1: Instalación Física

**1. ¿Por qué es importante evitar obstáculos entre los APs en una red Mesh?**<br />
Es crucial porque los nodos Mesh se comunican entre sí de forma inalámbrica (backhaul). Los obstáculos físicos (árboles, muros, edificios) causan atenuación de la señal, lo que reduce drásticamente el ancho de banda, aumenta la latencia y puede provocar desconexiones entre los nodos, afectando a toda la red.

**2. ¿Cuáles son las ventajas de usar PoE en la instalación de APs en exteriores?**
* **Simplicidad:** Permite enviar datos y energía eléctrica a través de un solo cable Ethernet, reduciendo el costo y tiempo de instalación.
* **Seguridad:** Evita la necesidad de instalar enchufes eléctricos en exteriores, los cuales son vulnerables a la lluvia y al clima.
* **Gestión centralizada:** Permite reiniciar el equipo de forma remota apagando y encendiendo el puerto desde un switch PoE.

## Paso 2: Configuración Inicial del AP

**3. ¿Por qué es recomendable usar una IP estática en el AP?**<br />
Una IP estática garantiza que el dispositivo de administración (controlador) siempre sepa dónde encontrar el AP en la red. Si se usara DHCP y la IP cambiara, podrías perder temporalmente la capacidad de monitorear o configurar el equipo, dificultando la resolución de problemas.

**4. ¿Qué factores considerar al elegir el canal Wi-Fi en exteriores?**
* **Interferencia de otras redes:** Se debe realizar un escaneo de radiofrecuencia (RF) para elegir canales menos saturados.
* **Canales DFS (Selección Dinámica de Frecuencias):** En exteriores (especialmente en 5 GHz), el uso de canales DFS está regulado porque pueden interferir con radares meteorológicos o de aviación. Si el AP detecta un radar, cambiará de canal abruptamente.
* **Canales no superpuestos:** En la banda de 2.4 GHz, usar estrictamente los canales 1, 6 u 11.

## Paso 3: Configuración de Mesh

**5. ¿Cuál es la función del nodo principal (Root Node) en una red Mesh?**<br />
El nodo principal es el que está conectado físicamente por cable a la red principal (switch/router) y al acceso a Internet. Actúa como el "puente" o puerta de enlace entre el entorno inalámbrico Mesh y la red cableada tradicional.

**6. ¿Por qué es importante tener una banda dedicada para el backhaul en redes Mesh?**<br />
En los sistemas Mesh de banda dual, si el AP usa la misma frecuencia para conectarse con los usuarios y para comunicarse con el nodo principal, el ancho de banda se reduce a la mitad (efecto *half-duplex*). Una banda dedicada (como una segunda radio de 5 GHz) permite que la comunicación entre nodos no compita con el tráfico de los usuarios, manteniendo la velocidad alta.

## Paso 4: Pruebas y Validación

**7. ¿Cómo se puede identificar si hay interferencias en la red Mesh?**
* Mediante herramientas de análisis Wi-Fi (como WiFiman o WiFi Analyzer) observando la saturación del espectro.
* Alta latencia (ping elevado) o pérdida de paquetes al comunicarse entre dispositivos.
* En el panel del controlador de red, revisando los porcentajes de "Utilización del Canal" y "Reintentos de Tx/Rx".

**8. ¿Qué hacer si un nodo Mesh tiene mala conectividad con el principal?**
* Reubicar el nodo para mejorar la línea de vista o reducir la distancia física.
* Verificar si hay nuevas fuentes de interferencia física o de radiofrecuencia.
* Añadir un nodo Mesh intermedio que sirva como puente (salto) para acortar la distancia.

## Paso 5: Seguridad y Mantenimiento

**9. ¿Qué riesgos implica no cambiar la contraseña de administración del AP?**<br />
Dejar las credenciales por defecto (ej. admin/admin) permite que cualquier usuario conectado a la red (o desde afuera si está expuesto) tome control total del dispositivo, cambie configuraciones, intercepte tráfico o desactive la red por completo.

**10. ¿Por qué es importante mantener el firmware del AP actualizado?**<br />
Las actualizaciones corrigen vulnerabilidades de seguridad descubiertas recientemente, mejoran la estabilidad del dispositivo, optimizan el rendimiento de radiofrecuencia y añaden compatibilidad con nuevas funciones del controlador.