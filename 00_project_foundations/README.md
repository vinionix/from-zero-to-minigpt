# Project Foundations

Esta fase prepara a base técnica usada por todos os mini projetos do repositório.

## Requisitos

- Python 3.12+
- `venv`
- `pip`

## Criar o ambiente virtual

```bash
python3 -m venv .venv
```

### Ativação no Bash/Zsh

```bash
source .venv/bin/activate
```

### Ativação no Fish

```fish
source .venv/bin/activate.fish
```

## Instalar dependências

Para executar apenas as dependências principais do projeto:

```bash
pip install -r requirements.txt
```

Para desenvolvimento, testes e notebooks:

```bash
pip install -r requirements-dev.txt
```

`requirements-dev.txt` inclui automaticamente as dependências de `requirements.txt`.

## Executar os testes

Com o ambiente virtual ativo:

```bash
pytest
```

O `pytest.ini` define `tests/` como diretório oficial de testes e usa os padrões `test_*.py` para arquivos e `test_*` para funções.

## Dependências iniciais

### Projeto e experimentos

- NumPy
- Matplotlib

### Desenvolvimento

- pytest
- Jupyter

As primeiras fases evitam frameworks que escondam os cálculos fundamentais. PyTorch será introduzido depois que gradientes e mecânica de redes neurais tiverem sido estudados e implementados de forma explícita.

## Padrão dos mini projetos

Cada módulo deve conectar teoria, matemática, implementação, teste e evidência experimental. O template oficial está em:

```text
docs/templates/MINI_PROJECT_README.md
```

As seções mínimas são:

1. objetivo;
2. problema e pré-requisitos;
3. matemática e exemplo manual;
4. implementação;
5. testes;
6. experimentos;
7. resultados;
8. limitações;
9. referências;
10. critério de conclusão.

Uma etapa não é considerada concluída apenas porque o código executa.

## Padrão dos experimentos

A convenção completa está em `experiments/README.md` e o relatório-base em:

```text
docs/templates/EXPERIMENT_REPORT.md
```

Identificadores seguem:

```text
exp_NNN_<descricao-curta>
```

A seed padrão é `42` quando há aleatoriedade, mas todo relatório deve registrar a seed efetivamente utilizada. Se a execução for determinística, registre `N/A`.

Todo experimento deve declarar previamente a pergunta, hipótese e métricas e registrar dataset/entrada, configuração, comandos, resultados observados, limitações e artefatos relevantes.

Resultados negativos, erros e hipóteses rejeitadas também devem permanecer documentados.

O critério central é reprodutibilidade: outra pessoa deve conseguir reconstruir o experimento apenas com a documentação e os arquivos versionados.

## Reprodutibilidade do ambiente

A pasta `.venv/` não é versionada. O ambiente deve ser reconstruído a partir dos arquivos de dependências, permitindo que cada máquina crie um ambiente compatível com seu próprio sistema operacional e arquitetura.

## Validação automática

O workflow `.github/workflows/tests.yml` executa a instalação das dependências e o `pytest` em um ambiente Linux limpo com Python 3.12 a cada push ou pull request para `main`. Isso funciona como validação contínua da receita de instalação do projeto.

## Check de sanidade

O projeto inclui `tests/test_sanity.py` para validar que a infraestrutura de testes está operacional. O teste não representa lógica de IA; ele apenas comprova que o `pytest` consegue descobrir e executar testes com um único comando.
