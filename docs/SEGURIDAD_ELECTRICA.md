# Seguridad eléctrica y control físico — SimuPLC

> **ADVERTENCIA: RIESGO DE DESCARGA ELÉCTRICA, ARRANQUE INESPERADO Y LESIONES GRAVES.**

SimuPLC es una herramienta educativa de simulación y programación. Sus funciones de conexión y programación de Arduino pueden accionar dispositivos físicos. **No utilice SimuPLC ni Arduino como sistema de protección, parada de emergencia, enclavamiento de seguridad o controlador de seguridad industrial.**

Antes de conectar o energizar cualquier equipo, una persona técnicamente competente debe verificar la tensión, el cableado, las protecciones, el aislamiento eléctrico, el estado seguro al reiniciar y ante pérdida de comunicación, y los procedimientos de bloqueo/etiquetado que correspondan. No realice conexiones sobre circuitos energizados. Los motores y otras cargas peligrosas requieren protecciones físicas independientes, incluido un medio de parada de emergencia apropiado. Una falla térmica simulada en HMI no sustituye la protección real del motor.

**Texto sugerido para confirmación previa a Programar Arduino / Conectar control físico:**

«⚠️ Advertencia de seguridad eléctrica. La programación y el control de equipos físicos pueden ocasionar descarga eléctrica, arranque inesperado, lesiones y daños materiales. Utiliza esta función únicamente con conocimientos técnicos suficientes, conexiones verificadas y protecciones físicas independientes. SimuPLC y Arduino son herramientas educativas y no sustituyen sistemas de seguridad industrial. [ ] He leído y comprendido la advertencia. [Cancelar] [Continuar]»

La aceptación no debe permitir omitir protecciones ni reemplazar las validaciones técnicas. Registrar la versión del aviso aceptado, y volver a solicitar aceptación cuando cambie sustancialmente. No bloquear las funciones de simulación offline por este aviso.

## Condiciones de uso — propuesta sujeta a revisión legal

SimuPLC se ofrece como herramienta educativa para simulación, programación y prácticas de automatización. El uso con dispositivos físicos requiere formación técnica, evaluación de riesgos y protecciones independientes apropiadas. El usuario debe comprobar conexiones, tensiones, compatibilidad de componentes y medidas de protección antes de energizar equipos. SimuPLC no está diseñado ni certificado como controlador de seguridad industrial. Estas condiciones no excluyen derechos del consumidor ni responsabilidades que no puedan limitarse conforme a la legislación aplicable. El texto debe ser revisado por asesoría legal antes de publicarse como términos contractuales.

## Criterios de aceptación para implementar en la interfaz

- Mostrar advertencia antes de **Programar Arduino** y antes de habilitar **control físico**, sin impedir la simulación virtual.
- Requerir aceptación explícita y ofrecer cancelar; no dar por aceptado mediante silencio.
- No iniciar una programación ni activar salidas mientras el diálogo está abierto.
- Evitar que cerrar el diálogo o navegar entre vistas eluda la confirmación.
- Verificar y probar estado seguro ante desconexión USB, reinicio de Arduino, pérdida de comunicación y reconexión; las salidas peligrosas deben contar con protecciones físicas independientes.
- Añadir acceso visible a Seguridad eléctrica y Términos de uso.
- Probar Android/OTG y PC/USB con hardware de prueba de baja tensión antes de utilizar motores.
