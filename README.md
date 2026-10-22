# cofetarie-ci

Reusable GitHub Actions workflows pentru proiectele cofetarie (auth-server, cookie-be, frontend).

## Workflows disponibile

- `java-ci.yml` — lint (Spotless) + test + build (Maven). Pentru proiecte Java/Spring Boot.

## Cum se folosește

În proiectul care consumă pipeline-ul, în `.github/workflows/ci.yml`:

​```yaml
jobs:
  ci:
    uses: <org>/cofetarie-ci/.github/workflows/java-ci.yml@main
    secrets: inherit
​```