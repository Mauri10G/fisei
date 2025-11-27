# Revisión bibliográfica: eCommerce y PrestaShop   
**Asignatura:** Manejo y Configuración del Software — SW-MyCS-APE-04  
**Herramienta asignada:** eCommerce — *PrestaShop*  
**Fecha:** 27 de noviembre de 2025

---

## 1. ¿Qué es eCommerce?
El comercio electrónico (eCommerce) es el conjunto de prácticas, tecnologías y plataformas que permiten la compra y venta de bienes y servicios a través de redes digitales. Incluye funciones como catálogo de productos, carrito de compra, pasarelas de pago, gestión de inventario, gestión de clientes (CRM), envío y logística, y analítica de ventas. Estas plataformas pueden ser SaaS (p. ej. Shopify) o de código abierto (p. ej. PrestaShop, WooCommerce, Magento). :contentReference[oaicite:0]{index=0}

---

## 2. ¿Qué es PrestaShop?
PrestaShop es una plataforma de comercio electrónico de código abierto orientada a tiendas online medianas y pequeñas que ofrece un sistema modular (módulos y temas), panel de administración, gestión de productos/categorías, y comunidad/marketplace de addons. Es extensible mediante módulos y temas, y puede desplegarse sobre una pila LAMP/PHP o en contenedores Docker. La documentación oficial describe su arquitectura modular y guías oficiales para desplegarlo con Docker Compose. :contentReference[oaicite:1]{index=1}

---

## 3. Características generales de plataformas eCommerce (aplicadas a PrestaShop)
- Gestión de catálogo: productos, variantes, atributos y categorías. :contentReference[oaicite:2]{index=2}  
- Carrito y checkout configurable (opciones de impuestos, envíos y pasarelas). :contentReference[oaicite:3]{index=3}  
- Extensibilidad: módulos (funcionalidades) y temas (apariencia). :contentReference[oaicite:4]{index=4}  
- Panel de administración con reportes y herramientas de marketing. :contentReference[oaicite:5]{index=5}  
- Multiidioma y multimoneda (característica nativa en muchas instalaciones). :contentReference[oaicite:6]{index=6}

---

## 4. Componentes de PrestaShop (arquitectura y elementos clave)
1. **Core (núcleo)**: lógica principal en PHP, controladores, modelos, servicios. :contentReference[oaicite:7]{index=7}  
2. **Módulos**: paquetes que añaden o modifican funcionalidades (pago, envíos, SEO, etc.). :contentReference[oaicite:8]{index=8}  
3. **Temas**: plantillas Twig/Smarty, CSS y assets para la presentación. :contentReference[oaicite:9]{index=9}  
4. **Base de datos**: normalmente MySQL/MariaDB para persistencia. :contentReference[oaicite:10]{index=10}  
5. **Frontend / Backoffice**: interfaz de tienda (clientes) y panel administrativo (gestión). :contentReference[oaicite:11]{index=11}  
6. **Marketplace (Addons)**: repositorio de módulos y temas oficiales. :contentReference[oaicite:12]{index=12}

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

