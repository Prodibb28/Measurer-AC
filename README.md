# Medidor de Consumo Eléctrico

Este proyecto implementa un medidor de consumo eléctrico utilizando un Arduino Uno. El código proporcionado realiza la medición de voltaje, corriente y potencia en un sistema eléctrico.

## Requisitos

- Arduino Uno
- Sensor de voltaje ZMPBT-101
- Sensor de corriente SCT-013
- Circuito sumador de voltaje LM358

## Configuración

1. Conecta el sensor de voltaje ZMPBT-101 al pin analógico A1 del Arduino Uno.
2. Conecta el sensor de corriente SCT-013 al circuito sumador de voltaje LM358.
3. Conecta la salida del circuito sumador de voltaje LM358 al pin analógico A0 del Arduino Uno.

## Uso

1. Carga el código en el Arduino Uno utilizando el IDE de Arduino.
2. Conecta el Arduino Uno a una fuente de alimentación adecuada.
3. Observa los resultados de la medición de potencia a través de la comunicación serial a una velocidad de 115200 baudios.

## Detalles del Código

- El código proporcionado utiliza una aproximación de sumatoria discreta para calcular la potencia promedio, la tensión eficaz, la corriente eficaz y el factor de potencia.
- Utiliza un circuito sumador de voltaje LM358 para elevar el voltaje de salida del sensor de corriente SCT-013 y hacerlo compatible con el ADC del Arduino Uno.
- El código actualmente no incluye la funcionalidad para determinar si el factor de potencia está en adelanto o en atraso.
- La determinación de la frecuencia de la red eléctrica aún no ha sido implementada en el código.
- El código puede optimizarse para mejorar el rendimiento y la eficiencia.

## Esquema de Conexiones

Se proporcionará un archivo de esquema de conexiones (formato PDF) en la carpeta "Esquema" del repositorio. Asegúrate de revisar el esquema para conectar correctamente los sensores y el circuito sumador de voltaje al Arduino Uno.

## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si encuentras algún error, tienes sugerencias de mejora o deseas agregar nuevas funcionalidades, por favor, crea un pull request o abre un issue en el repositorio.

## Licencia

Este proyecto se encuentra bajo una licencia Creative Commons [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.es). Consulta el archivo `LICENSE` para obtener más detalles.

La licencia Creative Commons Attribution 4.0 International (CC BY 4.0) permite a otros distribuir, remezclar, modificar y utilizar este proyecto, incluso con fines comerciales, siempre y cuando se les atribuya el crédito correspondiente.

Si deseas utilizar este proyecto o partes de él en tu propio proyecto, asegúrate de revisar y cumplir con los términos y condiciones de la licencia CC BY 4.0.

Estamos trabajando en desarrollar las siguientes características adicionales:
- Determinación del factor de potencia en adelanto o atraso.
- Determinación de la frecuencia de la red eléctrica.
- Optimización del código para mejorar el rendimiento.
- Actualización del esquema de conexiones.

Agradecemos cualquier contribución adicional para mejorar este proyecto. Si tienes ideas o sugerencias sobre cómo implementar estas características o cualquier otra mejora, no dudes en compartirlas.

