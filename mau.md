# Revisión bibliográfica: eCommerce y PrestaShop   
**Asignatura:** Manejo y Configuración del Software — SW-MyCS-APE-04  
**Herramienta asignada:** eCommerce — *PrestaShop*  
**Fecha:** 27 de noviembre de 2025

---

## 1. ¿Qué es eCommerce?
El comercio electrónico o eCommerce es la forma de comprar y vender productos o servicios a través de internet. Funciona como una tienda física pero todo ocurre en una página web o aplicación; las personas pueden explorar productos, hacer pedidos y pagar desde cualquier lugar y en cualquier momento.
El eCommerce se apoya en varias funciones básicas que permiten que una tienda digital trabaje de manera ordenada y segura. Entre las más comunes están:

- Catálogo de productos donde se muestran precios, fotos y descripciones
- Carrito de compras que permite guardar los artículos antes de pagar
- Métodos de pago en línea como tarjetas, transferencias o billeteras digitales
- Gestión de inventario para controlar las existencias y movimientos
- Registro de pedidos y seguimiento de envíos

Existen diferentes tipos de modelos de eCommerce; por ejemplo tiendas que venden directo al cliente, empresas que venden a otras empresas o plataformas donde los usuarios pueden vender entre sí. También hay distintas herramientas para crear una tienda; algunas son servicios listos para usar como Shopify y otras son de código abierto como PrestaShop que permiten personalización y control total.

El eCommerce es importante porque ayuda a llegar a más clientes, operar las 24 horas del día y reducir costos, por lo que muchos negocios lo utilizan para crecer y adaptarse a la economía digital actual.

---

## 2. ¿Qué es PrestaShop?
PrestaShop es una plataforma de comercio electrónico de código abierto que permite crear y administrar una tienda en línea de forma completa. Se instala en un servidor web y ofrece todas las herramientas necesarias para mostrar productos, gestionar pedidos, manejar pagos y administrar clientes. Una ventaja importante de PrestaShop es que es flexible y se puede modificar gracias a su estructura basada en módulos y plantillas, lo que permite adaptarlo a diferentes tipos de negocios sin necesidad de depender de un sistema cerrado.

Esta plataforma es muy usada a nivel mundial porque combina facilidad de uso con funciones avanzadas. Su panel de administración permite organizar productos, configurar métodos de pago, controlar inventario y revisar estadísticas de ventas. Además, al ser un software libre, los usuarios pueden instalarlo sin pagar licencias y personalizarlo según las necesidades de su proyecto, lo que la convierte en una opción accesible tanto para pequeños emprendimientos como para negocios en crecimiento. PrestaShop también cuenta con una comunidad activa que crea módulos, temas y guías, lo que facilita la resolución de problemas y la incorporación de nuevas funciones.

---

## 3. Características generales de plataformas eCommerce 
PrestaShop tiene varias características que la convierten en una plataforma completa para construir una tienda en línea. Entre sus características principales se encuentran:
- Panel de administración intuitivo para manejar productos, clientes y pedidos
- Plantillas y temas para modificar el diseño de la página
- Soporte para múltiples idiomas y monedas
- Integración con diferentes métodos de pago y servicios de envío
- Herramientas básicas de marketing y estadísticas de ventas
Estas características hacen que PrestaShop sea una plataforma flexible y capaz de adaptarse tanto a tiendas simples como a proyectos más avanzados.

---

## 4. Componentes de PrestaShop 
PrestaShop está formado por varios componentes que trabajan juntos para que la tienda pueda funcionar de manera ordenada. El núcleo del sistema está desarrollado en PHP y contiene la lógica principal, como la forma en que se manejan los productos, los pedidos y las configuraciones. A este núcleo se le pueden añadir módulos, que son pequeñas extensiones que permiten integrar funciones como pagos, envíos, reportes adicionales o herramientas de marketing.

También cuenta con un sistema de temas que define el diseño visual de la tienda, desde los colores hasta la estructura de las páginas. La base de datos, normalmente en MySQL o MariaDB, guarda toda la información importante como productos, clientes y pedidos. Por último, PrestaShop incluye dos partes visibles para el usuario: la tienda en sí, que es donde los clientes navegan y compran, y el panel de administración o back office, donde el dueño de la tienda gestiona todas las operaciones.

Algunos componentes clave son:
1. **Core (núcleo)**: lógica principal en PHP, controladores, modelos, servicios. :contentReference
2. **Módulos**: paquetes que añaden o modifican funcionalidades (pago, envíos, SEO, etc.). 
3. **Temas**: plantillas Twig/Smarty, CSS y assets para la presentación. :contentReference
4. **Base de datos**: normalmente MySQL/MariaDB para persistencia.
5. **Frontend / Backoffice**: interfaz de tienda (clientes) y panel administrativo (gestión). 
6. **Marketplace (Addons)**: repositorio de módulos y temas oficiales. 

Estos elementos permiten que la tienda sea personalizable y funcional tanto para el administrador como para los clientes.
---

## 5. Ventajas de usar PrestaShop / plataformas open-source
- **Control y personalización:** código accesible para adaptar la solución. :contentReference[oaicite:13]{index=13}  
- **Ecosistema de módulos y comunidad:** marketplace con módulos y soporte comunitario. :contentReference[oaicite:14]{index=14}  
- **Costos iniciales reducidos:** no hay licencias por el core (aunque sí inversión en hosting, desarrollo y módulos premium). :contentReference[oaicite:15]{index=15}  
- **Multiidioma y multimoneda nativos**, útil para tiendas internacionales. :contentReference[oaicite:16]{index=16}

---

## 6. Desventajas y limitaciones
- **Necesidad de conocimientos técnicos** para personalizaciones avanzadas y mantenimiento (seguridad, backups, optimización). :contentReference[oaicite:17]{index=17}  
- **Rendimiento**: una tienda con muchos módulos/muchos productos puede requerir optimizaciones (caché, infraestructura, CDN, tuning de MySQL). :contentReference[oaicite:18]{index=18}  
- **Costos ocultos:** módulos premium, temas, hosting y mantenimiento. :contentReference[oaicite:19]{index=19}

---

## 7. Aplicaciones prácticas y casos de uso
- Tiendas de nicho y PYMES que requieren control sobre su tienda y capacidad de expansión mediante módulos. :contentReference[oaicite:20]{index=20}  
- Proyectos educativos y prototipos para aprender eCommerce dado su modelo open-source y facilidad de despliegue (local o en contenedores). :contentReference[oaicite:21]{index=21}

---

## 8. Buenas prácticas para despliegue (breve)
- Usar entornos contenedorizados (Docker Compose) para separar servicios: app (PHP-FPM/Apache), base de datos (MySQL/MariaDB), cache (Redis opcional) y volúmenes persistentes. La documentación oficial recomienda Docker Compose para facilitar redes y volúmenes. :contentReference[oaicite:22]{index=22}  
- Hacer hardening: SSL, backups automáticos, actualización de dependencias y monitorización. :contentReference[oaicite:23]{index=23}

---

## 9. Evidencia empírica y comparativa (resultados de estudios)
Estudios comparativos y análisis de usabilidad coinciden en que PrestaShop es una de las soluciones open-source con mejores resultados en usabilidad para tiendas pequeñas/medianas en varias evaluaciones académicas recientes. Estos trabajos comparativos analizan consistencia, interactividad y facilidad de uso frente a alternativas como Magento o soluciones basadas en CMS+plugin. :contentReference[oaicite:24]{index=24}

---

## 10. Conclusión teórica
PrestaShop representa una opción sólida para eCommerce open-source: combina extensibilidad, comunidad y herramientas administrativas completas. Es adecuada para proyectos con recursos para gestionar hosting y personalizaciones; su principal reto es el mantenimiento y la optimización en tiendas de alta carga. Para proyectos académicos y PYMES, su ecosistema y la posibilidad de desplegar con Docker facilitan reproducibilidad y experimentación. :contentReference[oaicite:25]{index=25}

---

## 11. Bibliografía (seleccionada)
- PrestaShop Developer Documentation — Architecture / Themes / Docker. :contentReference[oaicite:26]{index=26}  
- M. Wijaszka, M. Dzieńkowski (2024). *A usability analysis of e-commerce systems (PrestaShop, Magento, Joomla/HikaShop)*. Journal / Conference. :contentReference[oaicite:27]{index=27}  
- ScitePress (2018). *Evaluating Open Source E-commerce Tools using OSSpal* (comparativo de Prestashop, Magento, WooCommerce, etc.). :contentReference[oaicite:28]{index=28}  
- Tutorial/boilerplate y guías de despliegue en Docker (artículos y guías prácticas). :contentReference[oaicite:29]{index=29}  
- Docker Compose — documentación oficial (uso de redes, volúmenes y servicios). :contentReference[oaicite:30]{index=30}

---

## 12. Anexo: Notas para la parte práctica del grupo
- Para la **implantación con Docker Compose** (tarea de Damian) revisar la guía oficial de PrestaShop para Docker y usar `docker-compose.yml` que incluya al menos servicios: `prestashop` (PHP/Apache), `db` (MySQL/MariaDB), volúmenes persistentes y redes internas. :contentReference[oaicite:31]{index=31}  
- Para la **implantación por CLI (Jonathan)** usar comandos `docker network create`, `docker run -d --name mysql ...`, y enlazar la app con `--link` o redes bridge; documentar cada comando ejecutado. :contentReference[oaicite:32]{index=32}  
- Para la **implantación en hipervisor (Andrés)** documentar creación de VM, versión de SO instalada, paquetes PHP, extensiones, MySQL, permisos y configuración de Apache/Nginx. :contentReference[oaicite:33]{index=33}

---

## 13. Observaciones finales
La investigación evidencia que PrestaShop es una alternativa válida para el proyecto de curso por su equilibrio entre funcionalidad y facilidad de despliegue; sin embargo, la atención en rendimiento y seguridad debe ser prioritaria en producción.

