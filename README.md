# Portafolio de Análisis de Algoritmos

Reportes de las prácticas del curso **Análisis de Algoritmos** del programa
Maestría en Ciencia de Datos e Información de INFOTEC.

🌐 **Sitio publicado:** https://marioqtop8308.github.io/portafolio-algoritmos/

## Estructura

```
.
├── _quarto.yml              # Configuración del Quarto Website
├── styles.css               # Tema visual personalizado
├── index.qmd                # Portada
├── unidad-6/
│   ├── index.qmd            # Práctica 6.6.1
│   ├── referencias.bib
│   └── datos/               # Posting lists comprimidos (.json.gz)
└── docs/                    # Sitio generado (servido por GitHub Pages)
```

## Cómo reproducir los reportes

Requiere [Julia 1.10](https://julialang.org/downloads/) y
[Quarto 1.4+](https://quarto.org/docs/get-started/).

```bash
# Clonar el repo
git clone https://github.com/marioqtop8308/portafolio-algoritmos.git
cd portafolio-algoritmos

# Instalar paquetes de Julia (una sola vez)
julia -e 'using Pkg; Pkg.add(["JSON", "CodecZlib", "Plots", "StatsPlots", "Statistics", "Random"])'

# Renderizar el sitio completo
quarto render

# O renderizar una unidad específica
quarto render unidad-6/index.qmd
```

El resultado queda en `docs/` y puede abrirse con cualquier navegador.

## Sobre el autor

Mario Galván Rosales — estudiante de Maestría en Ciencia de Datos e Información, INFOTEC.
