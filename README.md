# Ferretería Central - POS (Android XML UI)

Maquetación de la interfaz gráfica en XML para Android del sistema de punto de venta (POS) y gestión de inventario de **Ferretería Central**, desarrollada para la evidencia **GA5-220501095-AA1-EV08** del programa *Análisis y Desarrollo de Software* (SENA).

## Sistema de diseño y estándares técnicos
- **Estética industrial:** Grafito (`#2C3E50`), Naranja Industrial (`#E67E22`) y Verde Éxito (`#1E7E34`), complementados con superficies claras y rojo técnico (`#C0392B`) para alertas.
- **Arquitectura y componentes:** `ConstraintLayout`, `RecyclerView`, `CardView`, `TextInputLayout` y recursos modulares (`colors.xml`, `dimens.xml`, `strings.xml`).
- **Ergonomía y accesibilidad:** Áreas táctiles mínimas de `48dp` (cumpliendo criterios WCAG / Android), botones principales de `56dp` y descripciones de contenido (`contentDescription`).

## Recursos y vistas creadas
- **Recursos base (`res/values`):**
  - `colors.xml`: Paleta cromática del sistema.
  - `dimens.xml`: Espaciados, tamaños táctiles, radios de borde y tipografía escalable.
  - `strings.xml`: Cadenas de texto de la aplicación y el mostrador.
- **Vistas y componentes (`res/layout`):**
  - `activity_login.xml`: Inicio de sesión con usuario, contraseña y acceso a registro.
  - `activity_pos_mostrador.xml`: Mostrador POS con búsqueda por SKU/código de barras, detalle de venta, subtotal, IVA (19%), total a pagar y acciones de cobro/cancelación.
  - `activity_inventario_stock.xml`: Gestión de inventario y stock con búsqueda y creación de productos.
  - `item_inventario_producto.xml`: Tarjeta de producto con SKU, nombre, stock disponible y alerta de stock bajo.
  - `dialog_procesar_pago.xml`: Ventana de cobro con monto total, método de pago, efectivo recibido, cambio/devuelta y confirmación de tiquete.
  - `fragment_reportes_venta.xml`: Resumen operativo con ventas del día, transacciones y alertas de reposición.
  - `activity_error_alerta.xml`: Pantalla de alerta o error del sistema con opciones de reintentar o volver al mostrador.

## Autora
- **Angie Melissa Quiroz Jimenez** — SENA, Análisis y Desarrollo de Software (Ficha 3388995).
