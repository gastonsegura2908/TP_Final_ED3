# SeMaKu – Sistema de Medición de Humedad y Temperatura en Suelo

**SeMaKu** es un sistema embebido desarrollado para la medición de humedad del suelo y temperatura ambiente, utilizando un microcontrolador **LPC1769 (ARM Cortex-M3)** y sensores analógicos. El sistema incluye comunicación UART bidireccional con una PC y una **interfaz gráfica en MATLAB** para visualización en tiempo real. Fue desarrollado como **Trabajo Práctico Final de Electrónica Digital III** (FCEFyN – UNC, 2023).

## 👨‍💻 Autores

- **Gastón Marcelo Segura** – [gastonsegura2908@mi.unc.edu.ar](mailto:gastonsegura2908@mi.unc.edu.ar)  
- **Federica Mayorga** – [federica.mayorga@mi.unc.edu.ar](mailto:federica.mayorga@mi.unc.edu.ar)  
- **Antonin Kulyk** – [antonin.kulyk@insa-lyon.fr](mailto:antonin.kulyk@insa-lyon.fr)

## 🎯 Objetivos

- Interfaz de captura de datos de humedad y temperatura utilizando sensores analógicos.
- Lectura mediante ADC en el microcontrolador LPC1769.
- Comunicación UART bidireccional con una PC.
- Visualización de datos en tiempo real mediante una GUI en MATLAB.

## ⚙️ Tecnologías y herramientas

- **Microcontrolador:** LPC1769 (Cortex-M3)
- **Lenguaje:** C (programación a bajo nivel sobre CMSIS)
- **Sensores:** LM35DZ (temperatura), FC-28 (humedad en suelo)
- **Comunicación:** UART a través de adaptador USB CP2102
- **Interfaz gráfica:** MATLAB
- **Interrupciones:** externas (botones), ADC, UART, Timer0, Timer1, Timer2
- **DMA:** habilitada para transferencia de datos sin intervención del CPU

## 🔧 Diseño del sistema

### Hardware
- 2 protoboards
- 1 placa LPC1769
- 1 sensor LM35DZ (temperatura)
- 1 sensor FC-28 (humedad de suelo)
- 3 LEDs indicadores (azul, rojo y blanco)
- 2 pulsadores
- 3 resistencias de 470Ω
- 1 convertidor USB a UART (CP2102)
- Cables y jumpers varios

### Funcionalidades implementadas
- Lectura de sensores por ADC0.4 y ADC0.5
- Conmutación de modos de operación mediante pulsadores
- Iluminación de LEDs según sensor activo
- Envío periódico de datos por UART a PC
- Interfaz MATLAB para visualización y control

## 📈 Resultados

### Interfaz gráfica (MATLAB)
- Visualización en tiempo real de los datos de humedad y temperatura.
- Indicador de modo activo (sensor activo).
- Soporte para PC y dispositivos compatibles con MATLAB.

### Pruebas realizadas
- Verificación de adquisición de datos
- Validación de comunicación UART
- Testeo de estabilidad del sistema con múltiples ciclos de medición

### Imágenes del sistema
- Sensores instalados
- LEDs indicadores activos
- Vista superior del montaje final

## ✅ Conclusiones

- Se logró una integración funcional de hardware y software en un entorno embebido.
- Se implementaron correctamente interrupciones, lectura ADC y comunicación UART.
- El uso de MATLAB aportó una capa visual muy útil para interpretación de los datos.
- Se exploraron conceptos avanzados como DMA y modos de ahorro de energía.

---

**Universidad Nacional de Córdoba**  
**Facultad de Ciencias Exactas**
