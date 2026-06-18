# Historias de Usuario - Expense-Keeper

## HU-01 — Registro de Gastos

**Como** usuario de Expense-Keeper,  
**quiero** registrar mis gastos indicando monto, categoría y fecha,  
**para** mantener un control organizado de mis movimientos financieros.

### Criterios de Aceptación (Formato Gherkin)

```gherkin
Escenario 1: Registro exitoso de un gasto
  Dado que el usuario está en el modal "Nuevo Movimiento"
  Cuando ingresa un monto mayor a cero, selecciona una categoría y una fecha válida
  Entonces el sistema guarda el gasto y lo muestra en el historial cronológico

Escenario 2: Intento de registro con monto inválido
  Dado que el usuario está en el modal "Nuevo Movimiento"
  Cuando ingresa un monto igual a cero o deja el campo vacío
  Entonces el sistema muestra un mensaje de error y no guarda el registro

Escenario 3: Intento de registro sin categoría
  Dado que el usuario está en el modal "Nuevo Movimiento"
  Cuando no selecciona ninguna categoría
  Entonces el sistema bloquea el envío y solicita que se elija una categoría
```

---

## HU-02 — Clasificación de Gastos por Categoría

**Como** usuario de Expense-Keeper,  
**quiero** clasificar mis gastos por categorías predefinidas,  
**para** identificar en qué rubro utilizo mi dinero con mayor frecuencia.

### Criterios de Aceptación (Formato Gherkin)

```gherkin
Escenario 1: Selección de categoría en el formulario
  Dado que el usuario está registrando un gasto
  Cuando despliega el selector de categorías
  Entonces visualiza opciones como Alimentos, Transporte, Entretenimiento, Salud y Otros

Escenario 2: Gasto registrado con categoría correcta
  Dado que el usuario seleccionó la categoría "Alimentos"
  Cuando guarda el gasto
  Entonces el historial muestra el movimiento etiquetado con "Alimentos"

Escenario 3: Gasto sin categoría asignada
  Dado que el usuario intenta guardar un gasto sin elegir categoría
  Cuando presiona el botón "Guardar"
  Entonces el sistema no procesa el registro y muestra un aviso de campo obligatorio
```

---

## HU-03 — Visualización del Historial Financiero

**Como** usuario de Expense-Keeper,  
**quiero** consultar el historial de mis movimientos financieros ordenado por fecha,  
**para** revisar y analizar mis gastos registrados en cualquier momento.

### Criterios de Aceptación (Formato Gherkin)

```gherkin
Escenario 1: Visualización del historial con registros existentes
  Dado que el usuario tiene gastos registrados
  Cuando navega a la pantalla de Historial
  Entonces visualiza una lista de movimientos ordenados del más reciente al más antiguo

Escenario 2: Información mínima por movimiento
  Dado que el historial contiene registros
  Cuando el usuario observa cada entrada
  Entonces cada movimiento muestra el monto, la categoría, el método de pago y la fecha

Escenario 3: Historial vacío
  Dado que el usuario no tiene gastos registrados
  Cuando navega a la pantalla de Historial
  Entonces el sistema muestra un mensaje indicando que aún no hay movimientos
```

---

## HU-04 — Gestión de Métodos de Pago

**Como** usuario de Expense-Keeper,  
**quiero** registrar y gestionar mis métodos de pago (efectivo y tarjetas),  
**para** identificar con qué instrumento financiero realizo cada gasto.

### Criterios de Aceptación (Formato Gherkin)

```gherkin
Escenario 1: Alta de nuevo método de pago
  Dado que el usuario está en la pantalla "Mis Tarjetas"
  Cuando completa el formulario con tipo de método, entidad financiera y últimos 4 dígitos
  Entonces el sistema guarda el método y lo lista en la pantalla de tarjetas registradas

Escenario 2: Asociar método de pago a un gasto
  Dado que el usuario tiene al menos un método de pago registrado
  Cuando registra un nuevo gasto en el modal "Nuevo Movimiento"
  Entonces puede seleccionar el método de pago desde un selector desplegable

Escenario 3: Intento de alta con campos incompletos
  Dado que el usuario está en el formulario de nuevo método de pago
  Cuando deja algún campo obligatorio vacío y presiona "Guardar"
  Entonces el sistema muestra un aviso de error y no registra el método
```
