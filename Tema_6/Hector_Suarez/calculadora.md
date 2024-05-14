# API de una calculadora online

**Recursos identificados:**
- Suma (sumar) Permite sumar N de números
- Resta (restar) Permite restar N de números
- Multiplicación (multiplicar) Permite realizar la operacion de multiplicación de dos numeros
- División (dividir) Permite realizar la operacion de división de dos numeros
- Radicación (raiz) Permite realizar la operacion de radicación de dos numeros
- Potenciación (potencia) Permite realizar la potenciación de dos numeros
- Detalle de operacion (detalle) Representa los datos de entrada y resultado de la operacion identificada por su ID


| Método HTTP | URI            | Query Params | Request Body | Response Body    | Códigos HTTP de respuesta |
|-------------|----------------|--------------|--------------|------------------|-------------------------|
| POST        | /api/sumar    | N/A          | ``{"n": [2, 2, 2, 2]}`` | ``{"operacion_id": 123}`` | 200, 400 |
| POST        | /api/restar    | N/A          | ``{"n": [2, 2, 2]}`` | ``{"operacion_id": 123}`` | 200, 400 |
| POST        | /api/multiplicar    | N/A          | ``{"multiplicando": 2, "multiplicador": 2}`` | ``{"operacion_id": 123}`` | 200, 400 |
| POST        | /api/dividir    | N/A          | ``{"dividendo": 2, "divisor": 2}`` | ``{"operacion_id": 123}`` | 200, 400 |
| POST        | /api/raiz    | N/A          | ``{"radicando": 2, "indice": 2}`` | ``{"operacion_id": 123}`` | 200, 400 |
| POST        | /api/potencia    | N/A          | ``{"exponente": 2, "base": 2}`` | ``{"operacion_id": 123}`` | 200, 400 |
| GET         | /api/detalle/{operacion_id}    | N/A          | N/A | ``{"resultado": 131, "entrada": {}}`` | 200, 400 |
