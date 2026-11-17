# DulceCuentas — Plataforma de autogestión financiera

Plataforma web orientada a la gestión financiera, inventario y pedidos para artesanas dulceras de El Carmen de Bolívar. El proyecto busca facilitar el control del negocio mediante una interfaz accesible, procesos claros y persistencia de datos en la nube.

## Propósito

DulceCuentas nace para apoyar la organización de emprendimientos tradicionales que manejan sus operaciones de forma manual, ayudando a:
- Separar y controlar ingresos y gastos del negocio.
- Registrar ventas y realizar cierres de caja.
- Administrar inventario y niveles de disponibilidad.
- Dar seguimiento a encargos y pedidos de clientes.

## Funcionalidades principales

### 1. Gestión multi-tienda y acceso por perfil
- Manejo de información independiente por emprendimiento.
- Carga inicial de perfiles y descarga bajo demanda de datos operativos para la sesión activa.

### 2. Gestión financiera y punto de venta
- Registro de ventas con carrito y actualización de inventario.
- Registro de gastos operativos categorizados.
- Cálculo de indicadores como ingresos, egresos y utilidad neta.
- Cierre de caja diario y exportación de reportes en formato CSV.

### 3. Control de inventario
- Catálogo de productos por tienda con precios y existencias.
- Alertas visuales de stock bajo.
- Actualización rápida de cantidades mediante reabastecimiento.

### 4. Gestión de encargos
- Registro de pedidos con datos del cliente, fecha de entrega y detalle.
- Seguimiento del estado del encargo y conversión a venta cuando corresponde.

## Arquitectura y tecnologías

| Capa | Tecnología | Uso principal |
| --- | --- | --- |
| Interfaz | HTML5, CSS3, Tailwind CSS | Estructura, estilos y diseño responsivo |
| Lógica de cliente | JavaScript (ES6+) | Gestión de estado, interacción, cálculos y exportación CSV |
| Datos y backend como servicio | Supabase (PostgreSQL) | Persistencia relacional y acceso a datos |
| Visualización | Chart.js, Lucide Icons | Gráficas e iconografía de interfaz |

## Modelo de datos (referencial)

- **profiles**: información del emprendimiento/perfil.
- **inventory**: productos, stock y precios por tienda.
- **transactions**: registro de ventas y gastos.
- **orders**: encargos y pedidos de clientes.
- **cash_cuts**: cierres de caja diarios.

## Ejecución local

1. Clona el repositorio (si aplica):
   ```bash
   git clone https://github.com/jhoning-21/dulcecuentas.git
   cd dulcecuentas
   ```
2. Abre `index.html` en el navegador o utiliza Live Server en VS Code.

## Autor

**Jhon Diego Garrido Guzman**  
Estudiante de Ingeniería de Sistemas — Universidad Cooperativa de Colombia  
GitHub: [@jhoning-21](https://github.com/jhoning-21)
