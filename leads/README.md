# Leads — B2B Cold Outreach Uruguay

Generados con Google Maps Places API v2 (filtro: >40 reseñas, sin website, Montevideo Uruguay).

## Resumen

| Nicho | Cantidad | Leads |
|-------|----------|-------|
| Roofers | 3 | [Ver roofers/roofer-1.md](roofers/roofer-1.md) |
| HVAC | 2 | [Ver hvac/hvac-1.md](hvac/hvac-1.md) |
| Dentistas | 5 | [Ver dentistas/dentista-1.md](dentistas/dentista-1.md) |
| Fotógrafos | 4 | [Ver fotografos/fotografo-1.md](fotografos/fotografo-1.md) |
| Pileteros | 3 | [Ver pileteros/pilatero-1.md](pileteros/pilatero-1.md) |
| Abogados | 2 | [Ver abogados/abogado-1.md](abogados/abogado-1.md) |

## Formato por Lead

Cada lead se guarda en `leads/[nicho]/[slug].md`:

```markdown
# [Nombre del Negocio]

**Dirección:** [Dirección]
**Reseñas:** [N] ★★★★
**Teléfono:** [Si está disponible]
**Plus Code:** [Plus Code para ubicación]
**Nicho:** [Nicho]
**Notas:** [Observaciones]
```

## Workflow

1. Consultar API de Maps → leads pendientes
2. Crear archivo en `leads/[nicho]/`
3. Generar landing page → `landings/[negocio]/index.html`
4. Deploy → GitHub Pages
5. WhatsApp outreach
