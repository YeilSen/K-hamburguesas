# K-Hamburguesas - Sistema Integral de E-Commerce y Gestión de Restaurante

Bienvenido al repositorio oficial de **K-Hamburguesas**, una plataforma web *Full-Stack* desarrollada en **Laravel 12**. 
Este proyecto no es solo un menú en línea, sino un sistema integral que abarca la experiencia de compra del cliente (B2C) y la gestión operativa e inteligencia de negocios del restaurante.

## Características Principales

El sistema está dividido en dos grandes módulos, diseñados con una arquitectura MVC y protegidos por un sistema de autenticación basado en roles (RBAC).

### 1. Experiencia del Cliente (Front-End)
* **Catálogo Dinámico y Multilingüe:** Menú interactivo con soporte para Español e Inglés (traducción de base de datos e interfaz).
* **Carrito de Compras AJAX:** Gestión de productos sin recargar la página, cálculo de subtotales, IVA y costos de envío dinámicos.
* **Pasarela de Pagos Segura:** Integración con la API de **Stripe** para procesar pagos con tarjeta de crédito/débito de forma segura.
* **Comprobantes Automatizados:** Envío de tickets digitales (Mailables) en formato Markdown al correo electrónico del cliente al confirmar el pago.
* **Seguridad y Privacidad:** Sistema de registro protegido, recuperación de contraseñas por token y cumplimiento básico de privacidad.

### 2. Gestión del Restaurante (Panel de Administración)
* **Dashboard de Inteligencia de Negocios:** Métricas en tiempo real utilizando `Chart.js` para visualizar:
  * Evolución histórica de ventas (Gráfica de área).
  * Top 5 de productos más vendidos (Gráfica de dona).
  * Demanda por horas / Horas Pico (Gráfica de barras).
* **Monitor de Cocina (KDS) y POS:** Flujo de trabajo en tiempo real para transicionar estados de pedidos (`Pendiente` -> `Preparando` -> `Listo` -> `Entregado`).
* **Gestión de Personal:** CRUD completo para administrar cuentas de empleados, asignación de roles (Cajero, Cocinero, Repartidor, Admin) y selección dinámica de avatares.

---

## Herramientas utilizadas

* **Back-End:** PHP 8.4, Laravel 12.x
* **Front-End:** Blade Templates, JavaScript Vanilla, Tailwind CSS
* **Base de Datos:** MySQL (Relacional)
* **Integraciones API:** Stripe (Pagos)
* **Herramientas de Build:** Vite, NPM

---
