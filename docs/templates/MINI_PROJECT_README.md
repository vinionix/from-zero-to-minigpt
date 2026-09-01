# <Nome do mini projeto>

## Objetivo

Descreva em poucas linhas o que esta etapa pretende compreender, implementar e validar.

## Problema

Explique qual problema técnico ou matemático motiva este mini projeto e por que ele aparece no caminho até um modelo de linguagem.

## Pré-requisitos

- Conceitos necessários antes de iniciar.
- Etapas/issues anteriores das quais este módulo depende.

## Matemática

Registre as equações, símbolos e intuições necessárias.

Para cada conceito importante:

1. defina os símbolos;
2. explique a ideia com palavras próprias;
3. resolva ao menos um exemplo pequeno manualmente;
4. relacione a matemática à implementação.

## Implementação

Descreva as decisões de implementação sem esconder o raciocínio atrás de bibliotecas de alto nível.

Inclua:

- estrutura dos arquivos;
- principais funções/classes;
- entradas e saídas esperadas;
- decisões de projeto relevantes.

## Testes

Documente o que precisa ser testado e por quê.

Inclua, quando aplicável:

- casos normais;
- casos-limite;
- invariantes matemáticos;
- comparação com cálculo manual;
- regressões de bugs encontrados.

Comando padrão:

```bash
pytest
```

## Experimentos

Liste os experimentos relacionados usando a convenção `exp_NNN_<descricao-curta>`.

| ID | Hipótese | Variável alterada | Métrica principal | Resultado |
|---|---|---|---|---|
| `exp_001_exemplo` | <hipótese> | <variável> | <métrica> | <resultado> |

Cada experimento deve possuir um relatório baseado em `docs/templates/EXPERIMENT_REPORT.md`.

## Resultados

Resuma o que foi demonstrado pela implementação e pelos experimentos.

Separe fatos observados de interpretações. Não trate um resultado esperado como comprovado sem evidência experimental.

## Limitações

Registre limitações conhecidas, simplificações, casos em que a implementação falha e perguntas ainda abertas.

Resultados negativos também fazem parte desta seção e não devem ser apagados apenas porque um experimento não confirmou a hipótese.

## Referências

Liste livros, artigos, vídeos, documentação e outras fontes efetivamente utilizadas.

## Critério de conclusão

- [ ] Consigo explicar o conceito com palavras próprias.
- [ ] Resolvi um exemplo pequeno manualmente quando há matemática envolvida.
- [ ] Implementei o conceito sem copiar cegamente.
- [ ] Os comportamentos importantes possuem testes.
- [ ] Executei e documentei ao menos um experimento quando aplicável.
- [ ] Seeds, configurações, dataset/entrada e métricas estão registrados.
- [ ] Resultados e limitações, inclusive negativos, estão documentados.
- [ ] Outra pessoa consegue reproduzir o trabalho a partir da documentação.
