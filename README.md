# Exercícios Práticos de Fundamentos de CI/CD – Entrega

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

## Como usar

1. **Crie o repositório** `ci-cd-exercicio` no GitHub e clone localmente.
2. **Copie estes arquivos** para a raiz do repo.
3. `git add . && git commit -m "Exercícios CI/CD" && git push origin main`
4. Acompanhe a aba **Actions** (CI) e **Releases** (CD) no GitHub.

## Dicas para os exercícios
- Simule falha no CI alterando `soma` para `return a + b + 1`, faça *push* e observe o pipeline falhar, depois corrija.
- Simule erro de estilo no `app.py` (ex.: remova um espaço) e confira o passo do linter falhar.
- Crie um branch `feature/nova-funcao`, adicione mudanças e abra um **Pull Request** para ver o pipeline no PR.
