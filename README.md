# EAFIT VP Estatutos

Sitio web para acceso a estatutos municipales construido con Quarto.

## Descripción

Este sitio web proporciona un acceso centralizado a los estatutos y documentos oficiales de diferentes municipios. Cuenta con una interfaz sencilla y sobria que presenta la información en formato de tabla.

## Características

- **Diseño sobrio**: Interface limpia y profesional
- **Tabla responsive**: Se adapta a diferentes tamaños de pantalla
- **Enlaces directos**: Acceso rápido a portales oficiales
- **Descarga de PDFs**: Enlaces directos a documentos
- **Estados visuales**: Indicadores del estado de cada documento
- **Compilación automática**: Deploy automático con GitHub Actions

## Estructura del proyecto

```
├── index.qmd              # Página principal
├── _quarto.yml           # Configuración de Quarto
├── styles.css            # Estilos personalizados
├── custom.scss           # Tema SCSS personalizado
├── docs/                 # Carpeta para PDFs
├── .github/workflows/    # Automatización GitHub Actions
└── README.md            # Este archivo
```

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
| Nombre Municipio | Departamento | [Portal Oficial](URL) | [📄 Descargar](docs/archivo.pdf) | Estado | Fecha |
```

### Cambiar estilos

- Modifica `styles.css` para cambios en CSS
- Modifica `custom.scss` para cambios en el tema base
- Actualiza `_quarto.yml` para configuración general

### Estados disponibles

- ✅ Activo: Documento actualizado y vigente
- ⚠️ En revisión: Documento en proceso de actualización  
- ❌ Pendiente: Documento pendiente por obtener

## Deploy

El sitio se despliega automáticamente en GitHub Pages cuando se hace push a la rama `main`. Los archivos generados se almacenan en la carpeta `docs`.

## Licencia

[MIT License](LICENSE)
