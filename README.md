# Medidor de Consumo Eléctrico

Este proyecto implementa un medidor de consumo eléctrico utilizando un Arduino Uno. El código proporcionado realiza la medición de voltaje, corriente y potencia en un sistema eléctrico.

## Requisitos

- Arduino Uno
- Sensor de voltaje
- Sensor de corriente

## Configuración

1. Conecta el sensor de voltaje al pin analógico A1 del Arduino Uno.
2. Conecta el sensor de corriente al pin analógico A0 del Arduino Uno.

## Uso

1. Carga el código en el Arduino Uno utilizando el IDE de Arduino.
2. Conecta el Arduino Uno a una fuente de alimentación adecuada.
3. Observa los resultados de la medición de potencia a través de la comunicación serial a una velocidad de 115200 baudios.

## Detalles del Código

- El código proporcionado utiliza una aproximación de sumatoria discreta para calcular la potencia promedio, la tensión eficaz, la corriente eficaz y el factor de potencia.
- Ajusta el periodo de muestreo en la variable `period` para adaptarlo a tus necesidades específicas.
- El código asume que la carga es puramente resistiva y puede no ser preciso en sistemas con cargas no lineales o reactivas.
- Si deseas realizar análisis más complejos, considera utilizar técnicas como la transformada de Fourier utilizando la biblioteca "arduinoFFT".

## Contribuciones

Las contribuciones a este proyecto son bienvenidas. Si encuentras algún error, tienes sugerencias de mejora o deseas agregar nuevas funcionalidades, por favor, crea un pull request o abre un issue en el repositorio.

## Licencia

Este proyecto se encuentra bajo una licencia Creative Commons [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.es). Consulta el archivo `LICENSE` para obtener más detalles.

La licencia Creative Commons Attribution 4.0 International (CC BY 4.0) permite a otros distribuir, remezclar, modificar y utilizar este proyecto, incluso con fines comerciales, siempre y cuando se les atribuya el crédito correspondiente.

Si deseas utilizar este proyecto o partes de él en tu propio proyecto, asegúrate de revisar y cumplir con los términos y condiciones de la licencia CC BY 4.0.

Espero que esta versión del README sea útil para tu proyecto. Recuerda personalizarlo y ajustarlo según las necesidades específicas de tu aplicación y asegurarte de cumplir con los términos de la licencia Creative Commons que elijas.
