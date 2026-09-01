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

## Reprodutibilidade

A pasta `.venv/` não é versionada. O ambiente deve ser reconstruído a partir dos arquivos de dependências, permitindo que cada máquina crie um ambiente compatível com seu próprio sistema operacional e arquitetura.

## Check de sanidade

O projeto inclui `tests/test_sanity.py` para validar que a infraestrutura de testes está operacional. O teste não representa lógica de IA; ele apenas comprova que o `pytest` consegue descobrir e executar testes com um único comando.
