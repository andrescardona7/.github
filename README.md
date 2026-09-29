# .github

Repositorio de configuración predeterminada a nivel de cuenta de GitHub.

Incluye:

- **Política de seguridad** (`SECURITY.md`): informe privado de vulnerabilidades
- **Plantillas de issues** (`.github/ISSUE_TEMPLATE/`): informe de error y solicitud de funcionalidad
- **Plantilla de pull request** (`.github/PULL_REQUEST_TEMPLATE.md`)
- **Flujo reutilizable de Gitleaks** (`.github/workflows/gitleaks.yml`) para detectar secretos

## Uso del flujo Gitleaks

Desde otro repositorio:

```yaml
jobs:
  scan:
    uses: andrescardona7/.github/.github/workflows/gitleaks.yml@main
```

## Contribuciones

Abra un issue con la plantilla adecuada o un pull request. Para seguridad, use el informe privado descrito en `SECURITY.md`.
