
## Actividad 4: Sistema de pedidos de componentes (DTD)

Crea un fichero `pedidos.dtd` que defina las reglas necesarias para validar un documento XML que represente pedidos de componentes informáticos en una tienda online.

No debes crear el XML, únicamente el **DTD externo**, pero este deberá ser capaz de validar correctamente un XML que siga exactamente las siguientes especificaciones.

---

### Estructura del documento

* El elemento raíz será `<pedidos>`
* Contendrá **uno o más** elementos `<pedido>`

---

### Pedido

Cada `<pedido>`:

* Debe tener un atributo obligatorio `id`
* Debe contener, en este orden:

  1. `<cliente>`
  2. `<fecha>`
  3. `<componentes>`
  4. `<precio-total>`

---

### Cliente

El elemento `<cliente>`:

* Debe contener, en este orden:

  * `<nombre>`
  * `<email>`

---

### Componentes

El elemento `<componentes>`:

* Debe contener **uno o más** elementos `<componente>`

---

### Componente

Cada `<componente>`:

* Debe tener un atributo obligatorio `tipo`
* Debe contener, en este orden:

  * `<nombre>`
  * `<marca>`
  * `<precio>`
  * `<cantidad>`

---

### Tipos de contenido

Los siguientes elementos deben contener únicamente texto:

* `<nombre>`
* `<email>`
* `<fecha>`
* `<marca>`
* `<precio>`
* `<cantidad>`
* `<precio-total>`

---

### Condiciones importantes

* Debes respetar **exactamente el orden de los elementos** indicado.
* Debes definir correctamente:

  * Elementos obligatorios
  * Elementos repetidos (`+`)
* Los atributos indicados deben ser **obligatorios** (`#REQUIRED`).
* No se deben permitir elementos adicionales a los especificados.

---

### Entrega

* Fichero: `pedidos.dtd`

---
