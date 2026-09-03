# Estructura de Medellín-GO!

## Base protegida
- `main`: versión estable restaurada. No se modifica durante las pruebas.
- `prototipo-pagos`: rama de desarrollo para cambios y validación.

## Capas del prototipo
1. **Interfaz**: modos Pasajero/Conductor, navegación, modales y alertas.
2. **Viaje**: solicitar, aceptar, iniciar y finalizar la carrera demo.
3. **Pagos simulados**: efectivo por defecto; tarjeta opcional con solo 4 dígitos.
4. **Liquidación**: dinero recibido, deuda del pasajero y saldo disponible del conductor.
5. **Retiros simulados**: cuenta simulada, monto pendiente y estados de retiro.
6. **Persistencia local**: únicamente datos de demostración mediante `localStorage`.

## Reglas de seguridad del prototipo
- No guardar números completos de tarjeta.
- No conectar bancos, Wompi ni pagos reales.
- No mezclar deuda del pasajero con saldo del conductor.
- No integrar cambios a `main` sin probar ambos recorridos.

## Orden de validación
1. Mapa y navegación.
2. Flujo de pasajero.
3. Flujo de conductor.
4. Efectivo completo.
5. Tarjeta simulada completa.
6. Calificación con estrellas.
7. Saldo y retiro simulado.
