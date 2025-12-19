# Space Shooter - Unreal Engine 5

Shooter espacial top-down desarrollado como proyecto académico en Unreal Engine 5, enfocado en supervivencia y acumulación de puntos.

---

## 🎮 Flujo del juego

### Pantallas y transiciones
- **Start Screen**: Pantalla inicial donde el jugador inicia la partida
- **Playing**: Zona de juego activa donde el jugador controla la nave
- **Game Over**: Pantalla de fin de partida al perder todas las vidas

Las transiciones entre pantallas son automáticas y sin interrupción del flujo de juego.

### Dinámica principal
El jugador controla una nave en un plano infinito, eliminando enemigos y evitando obstáculos para acumular la máxima puntuación antes de ser destruido.

---

## 🕹️ Controles

- **Movimiento**: Joystick analógico / WASD - desplazamiento libre en 8 direcciones
- **Disparo**: Botón accionable (gamepad/ratón) - disparo continuo automático
- **Mecánica de inmunidad**: El jugador tiene 2 segundos de inmunidad tras recibir daño

---

## 💥 Sistema de colisiones y daño

### Enemigos
- **Naves enemigas**: Causan daño al colisionar + disparan proyectiles contra el jugador
- **Meteoritos**: Causan daño solo por colisión (no disparan ni se destruyen)

### Jugador
- Sistema combinado de **vidas + salud**: El jugador posee 3 vidas
- Al recibir daño, pierde vida/salud y entra en estado de inmunidad
- Al perder todas las vidas → **Game Over**

---

## ⭐ Sistema de puntuación y daño

### Asignación de puntos
- **Enemigos destruidos**: +100 puntos por nave enemiga eliminada
- **Meteoritos evitados/destruidos**: +50 puntos

### Asignación de daño
- **Colisión con navío enemigo**: 1 daño al jugador
- **Impacto de proyectil enemigo**: 1 daño al jugador
- **Colisión con meteorito**: 1 daño al jugador
- **Recuperación**: El jugador regenera 1 punto de salud cada 5 segundos en juego

---

## 🛠️ Tecnología

- **Motor**: Unreal Engine 5
- **Programación**: Blueprints (visual scripting)
- **Input**: Enhanced Input System
- **UI**: UMG (Widgets)
- **Vista**: Top-down con cámara ortográfica fija

---

## 📋 HUD

El jugador visualiza en todo momento:
- **Vidas**: Contador de vidas restantes
- **Munición**: Disponibilidad de bombas especiales
- **Puntuación**: Puntos acumulados en la partida

---

## 🚀 Versión

Prototipo funcional - En desarrollo
