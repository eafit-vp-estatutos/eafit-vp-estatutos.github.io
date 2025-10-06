# Proyecto Estatuto Óptimo - Repositorio de Resultados

Sitio web para acceso a los resultados del proyecto de estatuto óptimo construido con Quarto.

## Descripción

Este sitio web es el repositorio oficial de los resultados del **Proyecto de Estatuto Óptimo** liderado por la **Gobernación de Antioquia** y el **Centro Valor Público de la Universidad EAFIT**. 

Proporciona acceso centralizado a los documentos, diapositivas e informes generados para diferentes municipios de Antioquia, presentando la información en una interfaz sencilla y sobria.

## Características del sitio

- **Diseño sobrio**: Interface limpia y profesional
- **Tabla responsive**: Se adapta a diferentes tamaños de pantalla
- **Múltiples formatos**: Acceso a diapositivas e informes por municipio
- **Enlaces web**: Links directos a portales municipales oficiales
- **Estados de progreso**: Indicadores visuales del estado de cada documento
- **Compilación automática**: Deploy automático con GitHub Actions
- **Información de contacto**: Datos del responsable del proyecto

## Municipios incluidos

El proyecto abarca los siguientes municipios de Antioquia:

- Alejandría (05021)
- Angelópolis (05036)
- Anorí (05040)
- Argelia (05055)
- Belmira (05086)
- Briceño (05107)
- Guadalupe (05315)
- Guatapé (05321)
- La Pintada (05390)
- Salgar (05642)
- Urrao (05847)

## Estructura del proyecto

```
├── index.qmd              # Página principal con tabla de resultados
├── _quarto.yml           # Configuración de Quarto
├── styles.css            # Estilos personalizados
├── custom.scss           # Tema SCSS personalizado
├── docs/                 # Carpeta para documentos PDF
│   ├── autores_about     # Información sobre autores del proyecto
│   ├── *-informe.pdf     # Informes detallados por municipio
│   └── *.pdf             # Diapositivas por municipio
├── .github/workflows/    # Automatización GitHub Actions
└── README.md            # Este archivo
```

## Tipos de documentos

Para cada municipio se proporcionan dos tipos de documentos:

1. **Diapositivas** (`.pdf`): Presentaciones ejecutivas de los resultados
2. **Informes** (`-informe.pdf`): Documentos detallados con análisis completo

## Desarrollo local

Para trabajar con este proyecto localmente:

1. Instala [Quarto](https://quarto.org/docs/get-started/)
2. Clona el repositorio
3. Ejecuta `quarto preview` para vista previa
4. Ejecuta `quarto render` para generar el sitio en la carpeta `docs`

## Personalización

### Agregar un municipio

Edita el archivo `index.qmd` y agrega una nueva fila a la tabla con la siguiente estructura:

```markdown
| Código | Nombre | Web | Diapositivas | Informe | Estado | Fecha |
| 05XXX | Municipio | [Link](URL) | [📄 Descargar](docs/municipio.pdf) | [📊 Descargar](docs/municipio-informe.pdf) | Estado | YYYY-MM-DD |
```

### Cambiar estilos

- Modifica `styles.css` para cambios en CSS
- Modifica `custom.scss` para cambios en el tema base
- Actualiza `_quarto.yml` para configuración general

### Estados disponibles

- ✅ **Revisado**: Documento actualizado y vigente
- ⚠️ **En revisión**: Documento en proceso de actualización  
- ❌ **Pendiente**: Documento pendiente por obtener o actualizar

## Contacto del proyecto

Para dudas, actualizaciones o información adicional:

📧 **Email**: [jmunozm1@eafit.edu.co](mailto:jmunozm1@eafit.edu.co)  
🌐 **Página web personal**: [www.jcmunozmora.co](https://www.jcmunozmora.co)

## Instituciones participantes

- **Gobernación de Antioquia**: Entidad líder del proyecto
- **Universidad EAFIT - Centro Valor Público**: Socio académico

## Deploy

El sitio se despliega automáticamente en GitHub Pages cuando se hace push a la rama `main`. Los archivos generados se almacenan en la carpeta `docs`.

## Licencia

[MIT License](LICENSE)
