# [PROJECT_NAME] Constitution
<!-- Constitucion web Plannia. Reemplaza [PROJECT_NAME] por el nombre del cliente o sitio. -->

## Core Principles

### I. Negocio primero
Todo sitio responde a un objetivo de negocio escrito y a un KPI principal medible (leads, ventas, reservas, llamadas). Ninguna pagina existe sin una accion objetivo, y ninguna accion objetivo existe sin un evento de analitica que la mida.

### II. Contenido antes que diseno, diseno antes que codigo
Se construye con contenido real aprobado por el cliente, nunca con texto de relleno. El diseno (wireframes, DESIGN.md y tokens) se aprueba antes de escribir codigo de paginas. La AI propone textos; el cliente decide.

### III. Accesibilidad WCAG 2.2 AA (NO NEGOCIABLE)
HTML semantico, un solo `h1` por pagina, contraste minimo 4.5:1 en texto normal y 3:1 en texto grande y controles, navegacion completa con teclado y foco visible, objetivos tactiles de al menos 24x24 px, `alt` en toda imagen y `label` en todo campo. Cero violaciones de axe en A y AA.

### IV. Rendimiento medible
Metas al percentil 75 en movil: LCP <= 2.5 s, INP <= 200 ms, CLS <= 0.1. Imagenes con dimensiones declaradas, formatos AVIF/WebP y lazy-load solo debajo del primer pantallazo. JavaScript solo donde HTML y CSS no alcanzan.

### V. Seguridad por defecto (OWASP Top 10:2025)
HTTPS con HSTS, encabezados de seguridad (CSP, X-Content-Type-Options, Referrer-Policy, Permissions-Policy), secretos solo en variables de entorno, validacion del lado del servidor y dependencias auditadas sin vulnerabilidades altas o criticas.

### VI. Lo mas simple que cumpla
El stack se elige por necesidad, no por moda: HTML/CSS/JS para demos, Astro para sitios de contenido, Next.js solo con login o datos en vivo, Shopify para comercio. Cada dependencia se justifica en el plan.

### VII. Sin estetica generica de AI
Cada sitio tiene una direccion estetica explicita en su DESIGN.md. Se evitan fuentes por defecto, degradados de plantilla, layouts identicos para cualquier giro y textos genericos.

## Estandares de entrega

- Estructura: `src/` se edita, `dist/` se genera; tokens de diseno en un solo archivo; archivos en kebab-case.
- Calidad automatizada: formateador, linter y verificacion de tipos en pre-commit; Lighthouse CI, axe con Playwright y pruebas end-to-end en cada pull request.
- SEO tecnico: `title` y meta description unicos, Open Graph, `sitemap.xml`, `robots.txt` correcto y datos estructurados JSON-LD segun el giro.
- Lanzamiento: dominio con HTTPS, version canonica, redirecciones 301, analitica verificada, Search Console con sitemap enviado y aviso de privacidad.

## Flujo de trabajo

- Las 9 fases: descubrimiento, arquitectura de informacion, stack, diseno, setup, desarrollo, QA, lanzamiento y mantenimiento. Cada fase cierra con su puerta.
- Una feature = una rama de Spec Kit con preview desplegado.
- Commits con Conventional Commits (`feat:`, `fix:`, `style:`, `refactor:`, `docs:`, `chore:`); un commit hace una sola cosa.
- Ninguna rama se integra sin CI en verde y revision.

## Definition of Done

Un sitio se entrega solo si cumple todo: objetivo y KPI medidos, contenido aprobado, Core Web Vitals en meta, WCAG 2.2 AA, responsive de 360 a 1440 px, probado en Chrome, Safari, Firefox y Edge, seguridad aplicada, SEO tecnico completo, codigo limpio con historial ordenado, README actualizado y cliente con accesos y plan de mantenimiento.

## Governance

Esta constitucion prevalece sobre cualquier otra practica dentro del proyecto. Las excepciones se documentan en el plan con su razon y fecha. Los cambios a la constitucion requieren aprobacion del responsable del proyecto y actualizar la version.

**Version**: [CONSTITUTION_VERSION] | **Ratified**: [RATIFICATION_DATE] | **Last Amended**: [LAST_AMENDED_DATE]
