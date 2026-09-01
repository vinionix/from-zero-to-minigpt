# Experimentos

Esta pasta registra experimentos reproduzíveis executados ao longo do projeto. O objetivo não é acumular outputs, mas manter uma trilha clara entre hipótese, configuração, execução, resultado e interpretação.

## Convenção de nomes

Cada experimento usa o formato:

```text
exp_NNN_<descricao-curta>
```

Exemplos:

```text
exp_001_learning_rate
exp_002_batch_size
exp_003_hidden_size
```

`NNN` é sequencial dentro do módulo. A descrição deve indicar a principal variável ou pergunta investigada.

## Organização

Quando um módulo exigir experimentos persistidos, use uma estrutura como:

```text
experiments/
└── <modulo>/
    └── exp_001_<descricao-curta>/
        ├── REPORT.md
        └── artifacts/
```

O `REPORT.md` deve seguir `docs/templates/EXPERIMENT_REPORT.md`.

Artefatos podem incluir gráficos, pequenos logs e resultados necessários para análise. Arquivos grandes, datasets brutos, ambientes virtuais e checkpoints pesados não devem ser versionados sem uma decisão explícita.

## Seed

A seed padrão do projeto é:

```text
42
```

Ela é apenas uma convenção para facilitar reprodutibilidade; não possui significado estatístico especial.

Todo experimento com aleatoriedade deve registrar a seed realmente utilizada. Quando não houver aleatoriedade, registre `N/A` e explique a razão.

Experimentos futuros que precisem avaliar variância não devem depender de uma única seed: nesse caso, registre todas as seeds e agregue os resultados de forma apropriada.

## Configurações obrigatórias

Todo relatório experimental deve registrar, quando aplicável:

- módulo e issue relacionada;
- data;
- versão do Python;
- hardware relevante;
- dataset ou entrada;
- seed;
- hiperparâmetros;
- arquitetura/configuração do modelo;
- comandos necessários para reprodução.

Não existe um conjunto fixo de hiperparâmetros para todas as fases. Registre apenas os que podem alterar o resultado daquele experimento.

## Métricas

As métricas devem ser escolhidas antes da execução e precisam responder à pergunta experimental.

Exemplos futuros incluem MSE para regressão, acurácia/BCE para classificação, loss/perplexity para modelos de linguagem e tempo de execução quando desempenho computacional fizer parte da pergunta.

Uma métrica não deve ser usada apenas porque é comum; seu papel precisa estar descrito no relatório.

## Resultados negativos

Resultados negativos são dados do projeto.

Se uma hipótese for rejeitada, uma configuração piorar o resultado ou uma execução falhar, isso deve permanecer registrado. O relatório deve distinguir:

- o que era esperado;
- o que foi observado;
- possíveis explicações;
- limitações que impedem uma conclusão mais forte.

Não apagar uma tentativa simplesmente porque ela não funcionou.

## Critério de reprodutibilidade

Um experimento só é considerado documentado quando outra pessoa consegue reconstruir a execução usando o relatório e os arquivos versionados do projeto.

Use o template:

```text
docs/templates/EXPERIMENT_REPORT.md
```
