# 🎓 App de Ventas Escolares & Punto de Despacho (PWA)

Una mini aplicación web interactiva y ligera para la gestión de ventas, control de pedidos y cierre de caja en eventos, ferias o cantinas escolares.

Diseñada para funcionar como **Progressive Web App (PWA)**, permitiendo su instalación directa en teléfonos Android y iPhone sin depender de tiendas de aplicaciones.

---

## 🚀 Características Principales

- **📱 Catálogo & Toma de Pedidos:** Selección rápida de productos por categorías (Comidas, Bebidas, Postres), ajuste de cantidades y selección de medio de pago (Efectivo, Transferencia, Tarjeta).
- **🎫 Generación de Vouchers con QR:** Crea automáticamente un número de orden único (`#ORD-XXXX`) y genera un código QR para que el cliente/alumno lo presente en el punto de entrega desde su celular.
- **📦 Pantalla de Despacho:** Vista dedicada para los alumnos encargados de entregar el pedido, con buscador por código de orden o caja y selector de estado (*Pendiente*, *Entregado*, *Cancelado*).
- **📊 Cierre de Caja:** Reporte diario detallado con desglose de totales recaudados por medio de pago y tabla resumida por cantidad de productos vendidos. Incluye botón para imprimir reporte.
- **🏷️ Gestión de Productos:** Permite crear, editar precios/imágenes y eliminar productos del menú directamente desde la app.
- **💻 Control de Cajas/Usuarios:** Selector superior para registrar transacciones por caja (*Caja 1*, *Caja 2*, *Caja 3*).
- **💾 Persistencia de Datos:** Todos los productos y pedidos se guardan automáticamente en el almacenamiento local del navegador (`localStorage`).

---

## 📁 Estructura del Proyecto

```text
app-ventas/
├── index.html       # Código principal (React + Tailwind CSS + QR Generator)
├── manifest.json    # Configuración PWA (Nombre, colores e íconos)
├── sw.js            # Service Worker para funcionamiento sin conexión (Cache)
└── README.md        # Documentación del proyecto
