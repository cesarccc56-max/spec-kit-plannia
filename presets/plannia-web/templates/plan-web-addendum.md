
## Decisiones web *(obligatorio, preset plannia-web)*

### Stack

- **Eleccion**: [HTML/CSS/JS | Astro | Next.js | Shopify | WordPress]
- **Por que**: [La necesidad concreta del spec que lo justifica]
- **Hosting**: [Vercel | Netlify | Cloudflare Pages | otro]
- **CMS**: [Ninguno | headless | WordPress] y quien lo usara
- **Dependencias agregadas**: [Cada una con su razon]

### Diseno

- **DESIGN.md**: [Ruta del archivo]
- **Direccion estetica en una frase**: [Por ejemplo "editorial sobrio con acentos calidos"]
- **Tokens**: [Ruta de tokens.css; paleta, tipografia, espaciado, radios]
- **Contrastes verificados**: [Si/No y herramienta]

### Analitica y marketing

| Evento | Disparador | Pagina | KPI que alimenta |
| --- | --- | --- | --- |
| [generate_lead] | [Envio de formulario] | [/contacto] | [Leads] |

- **Datos estructurados (JSON-LD)**: [Organization, LocalBusiness o subtipo, Product, Article, FAQPage, BreadcrumbList]
- **Consentimiento**: [Banner de cookies y Consent Mode si aplica]

### Presupuestos de calidad

| Metrica | Meta |
| --- | --- |
| LCP movil (p75) | <= 2.5 s |
| INP (p75) | <= 200 ms |
| CLS (p75) | <= 0.1 |
| Lighthouse accesibilidad | 100 |
| Lighthouse SEO | 100 |
| JavaScript inicial comprimido | <= 150 KB en sitios de contenido |
| Violaciones axe A/AA | 0 |

### Seguridad

- **Encabezados**: [CSP, HSTS, X-Content-Type-Options, Referrer-Policy, Permissions-Policy]
- **Secretos**: [Variables de entorno usadas, nunca en el repo]
- **Formularios**: [Validacion en servidor y antispam]

### Excepciones a la constitucion

- [Ninguna | principio, razon y fecha]
