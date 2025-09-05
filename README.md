# Exercícios Práticos de Fundamentos de CI/CD

Este repositório contém:
- `app.py` com as funções `soma` e `multiplica`.
- `test_app.py` com testes via `pytest`.
- `.flake8` com configuração mínima do linter.
- `build.sh` para empacotar `projeto.zip`.
- `.github/workflows/ci.yml` configurado para:
  - Lint (`flake8`)
  - Testes (`pytest`)
  - Build do artefato (`build.sh`)
  - **Release automático** com o `projeto.zip` em *push* no `main`.


## Dicas para os exercícios
- Simule falha no CI alterando `soma` para `return a + b + 1`, faça *push* e observe o pipeline falhar, depois corrija.
- Simule erro de estilo no `app.py` (ex.: remova um espaço) e confira o passo do linter falhar.
- Crie um branch `feature/nova-funcao`, adicione mudanças e abra um **Pull Request** para ver o pipeline no PR.
