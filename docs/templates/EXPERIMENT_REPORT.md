# Experimento — `exp_NNN_<descricao-curta>`

## Metadados

| Campo | Valor |
|---|---|
| Módulo | `<modulo>` |
| Issue relacionada | `#<numero>` |
| Data | `YYYY-MM-DD` |
| Seed | `42` ou valor utilizado |
| Python | `<versao>` |
| Ambiente | `<SO / CPU / GPU quando relevante>` |
| Dataset / entrada | `<identificador, caminho ou descrição>` |

Se o experimento não utilizar aleatoriedade, registre `Seed: N/A` e explique por quê.

## Pergunta experimental

Qual pergunta objetiva este experimento tenta responder?

## Hipótese

Registre a previsão **antes** de executar o experimento.

> Se `<variável>` mudar de `<A>` para `<B>`, espero `<efeito>` porque `<justificativa>`.

## Configuração

Registre todos os valores necessários para repetir a execução.

| Parâmetro | Valor |
|---|---:|
| `<parametro>` | `<valor>` |

Quando aplicável, inclua também:

- tamanho do dataset;
- divisão treino/validação/teste;
- número de épocas/steps;
- learning rate;
- batch size;
- arquitetura;
- inicialização;
- seed;
- versões relevantes das dependências.

## Métricas

Defina as métricas **antes** de olhar o resultado.

| Métrica | Por que será usada |
|---|---|
| `<metrica>` | `<motivo>` |

Não existe uma lista universal de métricas: cada experimento deve declarar apenas as que respondem à pergunta experimental.

## Procedimento

Descreva os passos necessários para reproduzir o experimento, incluindo os comandos executados.

```bash
# comando(s) de reprodução
```

## Resultados

Registre valores observados, tabelas e artefatos gerados.

| Execução / configuração | Resultado |
|---|---:|
| `<config>` | `<valor>` |

### Artefatos

Liste caminhos para gráficos, logs, checkpoints ou outros arquivos relevantes.

- `<caminho-do-artefato>`

## Resultado esperado vs. observado

**Esperado:** <o que a hipótese previa>

**Observado:** <o que realmente ocorreu>

## Falhas e resultados negativos

Documente erros, hipóteses rejeitadas, execuções que não melhoraram a métrica e comportamentos inesperados. Não remova resultados só porque foram ruins.

## Interpretação

Explique o que os resultados permitem concluir e, igualmente importante, o que eles **não** permitem concluir.

Diferencie observação de inferência.

## Limitações

Registre fatores que podem reduzir a validade ou a generalização do experimento, como dataset pequeno, poucas repetições, hardware, ruído, métrica imperfeita ou ausência de baseline.

## Próximo experimento

Qual pergunta ficou aberta ou qual variável deveria ser investigada em seguida?

## Checklist de reprodutibilidade

- [ ] Pergunta e hipótese foram registradas.
- [ ] Seed ou ausência de aleatoriedade foi registrada.
- [ ] Dataset/entrada está identificado.
- [ ] Configuração e hiperparâmetros estão completos.
- [ ] Métricas estão definidas.
- [ ] Comandos de execução estão documentados.
- [ ] Resultados observados foram registrados.
- [ ] Resultados negativos/falhas foram preservados.
- [ ] Artefatos relevantes possuem caminhos identificáveis.
