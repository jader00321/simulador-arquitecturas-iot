🚦 Simulador de Arquitecturas IoT en Ciudades Inteligentes (Smart City)

📌 Descripción del Proyecto

Este proyecto es un simulador interactivo de telemetría y tráfico vehicular desarrollado para el curso de Sistemas Distribuidos. Su objetivo es demostrar de forma visual y matemática las diferencias críticas de rendimiento, latencia y tolerancia a fallos entre dos paradigmas de red:

Arquitectura Centralizada (Cloud + RPC Síncrono): Los sensores envían datos crudos a un servidor remoto, generando cuellos de botella y timeouts.

Arquitectura Distribuida (Edge Computing + MOM Asíncrono): Gateways locales procesan la información en milisegundos, resolviendo la exclusión mutua localmente y actualizando la nube en segundo plano.

🚀 Enlace en Vivo (Live Demo)

Puedes ejecutar y probar el simulador directamente desde el navegador, sin necesidad de instalación, haciendo clic en el siguiente enlace:
👉 https://jader00321.github.io/simulador-arquitecturas-iot/ 

⚙️ Características Técnicas

Motor de Físicas 2D (Kinematic Clamping): Algoritmos de colisión y frenado estricto para evitar el apilamiento de vehículos, asegurando un comportamiento vehicular realista.

Telemetría en Tiempo Real (Sparklines): Monitoreo del Round-Trip Time (RTT), simulando latencia de red con fluctuaciones aleatorias y picos de estrés.

Control de Ejecución Frame-by-Frame: Sistema de pausa y avance paso a paso para el análisis detallado del bloqueo de hilos (Thread Blocking) durante peticiones síncronas.

Comunicación Asíncrona: Representación visual del encolamiento de mensajes y transmisión en background (Middleware Orientado a Mensajes).

📊 Instrucciones de Uso

Selecciona la Densidad de Tráfico en el menú superior (Bajo, Normal, Extremo).

Para evaluar la arquitectura tradicional, presiona "Inyectar Tráfico" en el panel izquierdo (Cloud). Observarás cómo el RTT se dispara, ocurre un Timeout por espera síncrona y la intersección colapsa.

Para evaluar la arquitectura distribuida, presiona "Inyectar Tráfico" en el panel derecho (Edge). El Gateway local resolverá el tráfico en 4ms y la transmisión a la nube se realizará de forma asíncrona.

👨‍💻 Autor

Julio Angello Vasquez Navarro

Código: U22229509

Universidad Tecnológica del Perú (UTP)

Curso: Sistemas Distribuidos
