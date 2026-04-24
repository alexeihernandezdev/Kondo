# Kondo (Sistema para condominios)

---

## 1) ¿En que consiste?

es una plataforma SaaS (Software as a Service) diseñada para transformar la administración de condominios y urbanizaciones cerradas en Venezuela. A diferencia de los sistemas contables tradicionales, Kondo se enfoca en resolver la fricción financiera causada por la economía multimoneda (Bs/USD), automatizando la conciliación de pagos y devolviendo la transparencia a los copropietarios a través de una interfaz moderna, rápida y accesible desde cualquier dispositivo.

## 2) El Problema (Contexto Venezuela 2026)

En Venezuela, la gestión de condominios enfrenta tres retos críticos:

- Caos Multimoneda: La necesidad de cobrar en Bolívares a tasa oficial, pero presupuestar y pagar proveedores en Dólares, genera desajustes financieros y pérdidas por indexación.

- La "Selva de Captures": Los administradores pierden horas verificando manualmente pagos móviles, transferencias y Zelles recibidos por WhatsApp, lo que facilita errores y fraudes.

- Crisis de Confianza: La falta de acceso en tiempo real a las facturas y estados de cuenta genera conflictos entre vecinos y juntas directivas.

## 3) La Solución: ¿Qué hace Kondo?

Kondo actúa como un núcleo inteligente que conecta la cuenta bancaria del condominio con el bolsillo del vecino:

- Motor de Indexación Automática: Integra la tasa del BCV en tiempo real para calcular alícuotas y deudas, asegurando que el condominio no pierda valor frente a la inflación.

- Módulo de Conciliación "Smart-Check": Un sistema que procesa los reportes de pago de los vecinos, valida referencias bancarias duplicadas y organiza la "cola de aprobación" para el administrador.

- Portal de Transparencia Total: Los residentes cuentan con una PWA (Progressive Web App) donde pueden ver su deuda, descargar recibos y, lo más importante, auditar los gastos del condominio viendo fotos de las facturas reales.

- Comunicación Omnicanal: Automatiza el envío de avisos de cobro y recordatorios de mora a través de WhatsApp y correo electrónico.

## 4) Stack Tecnológico

Para garantizar la máxima velocidad y seguridad de los datos:

- Frontend: Next.js (React) para una experiencia de usuario fluida y carga instantánea (Optimizado para el internet de Venezuela).

- Backend: FastAPI (Python) para un procesamiento de datos robusto y scripts de automatización (Scraping de tasas y bots de notificación).

- Base de Datos: PostgreSQL para integridad financiera total.

- Infraestructura: Alojamiento en la nube con redundancia y copias de seguridad diarias.

## 5) Propuesta de Valor (Por qué Kondo)

Para el Administrador: Reduce el trabajo manual en un 70%. Elimina el uso de hojas de Excel propensas a errores.

Para el Vecino: Facilidad para reportar pagos en 30 segundos desde su celular y la tranquilidad de saber exactamente en qué se gasta su dinero.

Para la Comunidad: Reduce la morosidad mediante recordatorios automáticos y mejora la convivencia a través de la claridad de cuentas.

## 6) Visión 2026

Kondo no solo busca ser un software de cobranza, sino convertirse en el sistema operativo de las viviendas en venezuela.

---

## Especificaciones

### Módulo de Login

Contará con un modulo login en el que hay 3 tipos de usuarios:

- Superusuario: Maneja las cuentas de las residencias (Gestion de cuentas)
- Admin: sería dato por un nombre de cuenta, y esta será la encargada, de crear los gastos, validar pagos
- Usuario: Será dada por un correo electrónico, un usuario podria pertenecer a varios condominios. Puede subir su comprobante de pago. ver cuanto debe. entre otras cosas

#### Caracteristicas

- Se debe poder recuperar contrasena, cambiar contrasena, hacer login.
- Superusuario tendra una vista distinta enfocada a la gestion de las cuentas de residencias.
- Una cuenta de admin solo gestiona una residencia/condominio
- Una cuenta de usuario
- Arquitectura Multitenant, tablas compartidas pero con identificador

###
