
## Reglas web para tareas *(obligatorio, preset plannia-web)*

- Cada tarea termina con su **criterio de salida verificable** (la prueba, metrica o revision que la valida), no con "hecho".
- Orden de construccion: tokens y estilos base, layout global, componentes con todos sus estados, paginas con contenido real, interactividad y despues integraciones.

## Fase QA *(obligatoria antes de mostrar al cliente)*

- [ ] TQA-01 Lighthouse movil en el preview: rendimiento >= 90, accesibilidad 100, SEO 100
- [ ] TQA-02 axe con Playwright en todas las paginas: 0 violaciones A/AA
- [ ] TQA-03 Navegacion completa solo con teclado y foco visible
- [ ] TQA-04 Lector de pantalla (NVDA o VoiceOver) en 2 paginas clave
- [ ] TQA-05 Responsive en 360, 768, 1024 y 1440 px y en un celular real
- [ ] TQA-06 Chrome, Safari, Firefox y Edge actuales
- [ ] TQA-07 Validador HTML del W3C y revisor de enlaces: 0 errores
- [ ] TQA-08 Formularios: envio valido, envio con errores y llegada del lead
- [ ] TQA-09 Encabezados de seguridad (calificacion A o superior) y `npm audit` sin altas o criticas
- [ ] TQA-10 Titulos, descripciones, Open Graph y JSON-LD validados
- [ ] TQA-11 Eventos de analitica disparando en tiempo real
- [ ] TQA-12 Aprobacion escrita del cliente sobre el preview

## Fase lanzamiento

- [ ] TLA-01 Dominio, HTTPS y version canonica con redirecciones 301
- [ ] TLA-02 `robots.txt` permite rastreo y apunta a `sitemap.xml`; sin `noindex` heredado
- [ ] TLA-03 Search Console verificado y sitemap enviado
- [ ] TLA-04 Formularios probados en produccion
- [ ] TLA-05 Entrega al cliente: accesos, manual breve y README actualizado
