# action-e2e

Repo consumidor de teste da [fiscalspec/action](https://github.com/fiscalspec/action)
(spec 021 do monorepo, tasks T7/T8).

- `.github/workflows/fiscalspec.yml` — o `example.yml` da Action colado **tal como está**
  (aceite literal da T8: rodar verde na primeira tentativa num repo limpo).
- `.github/workflows/sarif.yml` — e2e da T7: `upload-sarif: true` com alerta visível em
  Security → Code scanning.
- `notas/devolucao.xml` — o XML de demonstração do CLI (conteúdo público, ADR 0005):
  devolução CFOP 1202 que a v1.51 rejeita com 321 (VC02-14).

Pré-requisito: secret `FISCALSPEC_API_KEY` (o ruleset é referenciado por id).
