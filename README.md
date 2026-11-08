# Señas LSM ✋

Reconocimiento de la dactilología (abecedario) de la **Lengua de Señas Mexicana (LSM)** con inteligencia artificial, directo en el navegador del celular.

Proyecto de Álvaro Márquez, intérprete de LSM.

## Cómo funciona

1. **Grabar**: haces cada letra frente a la cámara y la página guarda 30 ejemplos.
2. **Entrenar**: un clasificador de k vecinos más cercanos (k-NN) aprende de tus ejemplos y te dice qué letras confunde.
3. **Reconocer**: ves la letra en vivo y puedes deletrear palabras.

[MediaPipe Hand Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker) detecta 21 puntos de la mano. Esos puntos se centran en la muñeca, se escalan al tamaño de la palma y la mano izquierda se refleja para que ambas manos cuenten igual. Todo corre en el teléfono: tus ejemplos se guardan solo en tu navegador y nunca se suben a ningún servidor.

## Fases

- [x] **Fase 1:** abecedario sin movimiento
- [ ] **Fase 2:** letras con movimiento (J, K, Ñ, Q, X, Z, LL, RR)
- [ ] **Fase 3:** señas completas (saludos, números, días)
