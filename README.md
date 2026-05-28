# B2B Landing Pages — Uruguay

Landing pages generadas con AI para cold outreach B2B en Uruguay.

## Stack

- **LLM:** MiniMax (provider: minimax, modelo: MiniMax-M2.7)
- **Generación HTML:** Tailwind CSS via CDN
- **Hosting:** GitHub Pages (URL: `https://felidearmas.github.io/b2b-landing-pages/`)
- **Auth:** GitHub CLI (token `repo` scope)

## Estructura

```
b2b-landing-pages/
├── README.md
├── leads/                  # Datos de leads (CSV/JSON)
├── landings/              # Una subcarpeta por lead
│   └── [negocio]-[ciudad]/
│       └── index.html
└── scripts/               # Scripts de generación
```

## Metodología

1. Extraer leads desde Google Maps Places API v2 (filtro: >40 reseñas, sin website, Montevideo Uruguay)
2. Generar landing page con MiniMax (prompts en español + Tailwind)
3. Deploy a GitHub Pages
4. Outreach vía WhatsApp

## Leads Activos (19)

| Nicho | Cantidad |
|-------|----------|
| Roofers | 3 |
| HVAC | 2 |
| Dentistas | 5 |
| Fotógrafos | 4 |
| Pileteros | 3 |
| Abogados | 2 |

## Recursos

- Google Maps Places API v2: key OpenClaw (`AIzaSy...btAg`)
- Repo para acceder desde otra sesión: `felidearmas/b2b-landing-pages`

## Uso

```bash
# Clonar repo
git clone https://github.com/felidearmas/b2b-landing-pages.git

# Agregar landing page
cp -r landings/[negocio]/ /home/casa/hermes-research/iter_vault/b2b-landing-pages/landings/

# Push
cd b2b-landing-pages
git add .
git commit -m "feat: landing page [nombre]"
git push
```

## Activar GitHub Pages

Settings → Pages → Source: `main` branch, `/ (root)` → Save.

La URL será: `https://felidearmas.github.io/b2b-landing-pages/[landings/negocio/]`
