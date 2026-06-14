# Arquitectura de Datos y APIs - Expense-Keeper

Este documento define la estructura de datos (cargas útiles o *payloads*) y los métodos HTTP que utilizará el MVP para comunicar la interfaz de usuario con el servidor.

## 1. Registro de Gastos (Modal Nuevo Movimiento)
Esta interfaz recolecta la información de un egreso financiero. Como la acción principal es **crear** un nuevo registro en la base de datos, el método correspondiente es `POST`.

* **Endpoint:** `/api/v1/gastos`
* **Método HTTP:** `POST`
* **Carga útil (Request Body):** [Ver registro_gasto.json](./registro_gasto.json)
* **Respuesta Esperada (201 Created):** Confirmación de que el gasto fue guardado y el saldo fue actualizado.

## 2. Gestión de Métodos de Pago (Añadir Tarjeta/Efectivo)
Esta interfaz permite al usuario vincular una nueva cuenta o billetera. Dado que también implica **insertar** un nuevo recurso en el sistema, se utiliza el método `POST`.

* **Endpoint:** `/api/v1/metodos-pago`
* **Método HTTP:** `POST`
* **Carga útil (Request Body):** [Ver nuevo_metodo_pago.json](./nuevo_metodo_pago.json)
* **Respuesta Esperada (201 Created):** Confirmación de la vinculación del método de pago.

---

*Nota sobre consultas (GET):* Para las pantallas como el Historial Financiero (`view-history`) o el Dashboard (`view-home`), el sistema utilizará el método **`GET`** (ej. `GET /api/v1/gastos`), ya que estas vistas únicamente solicitan y consumen información sin alterar el estado del servidor.