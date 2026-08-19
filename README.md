# From Zero to MiniGPT

Construindo modelos de Inteligência Artificial do zero, desde a matemática básica até um pequeno modelo de linguagem baseado na arquitetura Transformer.

O objetivo deste repositório não é apenas utilizar bibliotecas prontas ou consumir APIs de modelos existentes. A proposta é compreender, implementar, testar e documentar os principais componentes envolvidos na construção de modelos modernos de IA — e depois conectar esse conhecimento à engenharia de sistemas com LLMs.

## Por que este projeto existe

Quero responder, na prática, a duas perguntas:

> Como um modelo de Inteligência Artificial aprende?

> O que é necessário para transformar esse conhecimento em um sistema de LLM testável, observável e seguro?

Por isso, o projeto não começa em Transformers. Ele reconstrói a base matemática e computacional necessária para chegar até eles com entendimento real.

## Método de trabalho

O projeto combina quatro frentes em cada etapa:

1. **Matemática:** compreender as operações e derivar as equações principais.
2. **Implementação:** transformar os conceitos em código, começando com Python e NumPy.
3. **Experimentação:** modificar parâmetros, provocar falhas e medir o comportamento.
4. **Documentação:** registrar resultados, limitações, erros e aprendizados.

Uma etapa só é tratada como concluída quando consigo explicar o conceito, resolver um caso pequeno manualmente, implementar, testar e analisar suas limitações.

## Roadmap

- [ ] Matemática básica para IA: aritmética, álgebra, funções, gráficos, potências e logaritmos
- [ ] Fundamentos matemáticos computacionais: vetores, matrizes, derivadas e probabilidade
- [ ] Regressão linear do zero
- [ ] Classificação e neurônio artificial
- [ ] Rede neural multicamada e backpropagation
- [ ] Modelos de linguagem simples
- [ ] Comparação entre RNN, GRU/LSTM, convolução causal e atenção
- [ ] Embeddings
- [ ] Self-attention e máscara causal
- [ ] Bloco Transformer decoder-only
- [ ] MiniGPT
- [ ] Fine-tuning e aprendizado por preferências
- [ ] API, RAG, ferramentas, avaliações e segurança
- [ ] Assistente técnico final para redes, infraestrutura ou cibersegurança

O roadmap detalhado e suas dependências estão na [issue #1](https://github.com/vinionix/from-zero-to-minigpt/issues/1).

## Fluxo técnico planejado

```text
Matemática básica
      ↓
Álgebra linear + derivadas + probabilidade
      ↓
Regressão e classificação
      ↓
MLP + backpropagation
      ↓
Modelos sequenciais
      ↓
Embeddings
      ↓
Self-attention
      ↓
Transformer decoder-only
      ↓
MiniGPT
      ↓
Post-training
      ↓
RAG + ferramentas + avaliações + segurança
```

## Fase -1 — Matemática básica para IA

Antes da álgebra linear, o projeto reconstrói a base necessária para ler e manipular fórmulas com segurança:

- aritmética, frações, razões e proporções;
- álgebra básica e equações;
- funções, plano cartesiano e leitura de gráficos;
- potências, raízes e notação científica;
- exponenciais e logaritmos;
- somatórios, índices, média e notação matemática;
- checkpoint prático aplicado a `y = wx + b`.

O código nessa fase serve para **validar a matemática**, não para substituir o raciocínio manual.

## Estrutura planejada

```text
from-zero-to-minigpt/
├── 00_project_foundations/
├── 01_basic_math/
├── 02_math_foundations/
├── 03_linear_regression/
├── 04_logistic_neuron/
├── 05_mlp_backpropagation/
├── 06_sequence_models/
├── 07_embeddings/
├── 08_self_attention/
├── 09_transformer/
├── 10_minigpt/
├── 11_post_training/
├── 12_llm_system/
├── docs/
├── experiments/
├── tests/
└── README.md
```

## Tecnologias

### Etapas iniciais

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- pytest

### Etapas avançadas planejadas

- PyTorch
- FastAPI
- Docker
- modelos abertos e bibliotecas de tokenização
- bancos vetoriais
- ferramentas de avaliação de LLMs

As primeiras implementações evitarão frameworks que escondam o cálculo dos gradientes. PyTorch será introduzido depois que os fundamentos forem implementados manualmente.

## Critério de conclusão

Uma etapa só será considerada concluída quando for possível:

- explicar a matemática com palavras próprias;
- calcular manualmente um exemplo pequeno;
- implementar o conceito sem copiar cegamente;
- criar testes para os comportamentos importantes;
- alterar parâmetros e analisar os resultados;
- identificar ao menos uma limitação;
- documentar erros, resultados e aprendizados.

Executar código copiado não representa a conclusão de uma etapa.

## Projeto final

O projeto final será um assistente técnico voltado para redes, infraestrutura ou cibersegurança. O sistema deverá combinar um modelo de linguagem com recuperação de documentação, ferramentas restritas, avaliações automatizadas, observabilidade e controles contra ataques como prompt injection.

## O que este repositório demonstra

Para quem estiver revisando o projeto como portfólio, os sinais principais que quero tornar visíveis são:

- evolução matemática aplicada à IA;
- implementação de fundamentos antes de abstrações de alto nível;
- capacidade de transformar teoria em experimentos reproduzíveis;
- criação de testes e critérios explícitos de conclusão;
- análise de falhas e limitações, não apenas de casos que funcionam;
- progressão de model internals para engenharia de sistemas com LLMs.

## Status e honestidade técnica

Este é um projeto **em andamento**. Itens do roadmap representam intenção de implementação, não funcionalidades já concluídas. O código, os testes e as notas de cada etapa são a evidência do que já foi realizado.

## Documentação

- [Technical Overview](docs/TECHNICAL_OVERVIEW.md) — visão de arquitetura, método de estudo, critérios de validação e direção técnica do projeto.

## Autor

Desenvolvido por Vinícius Fidelis.

- GitHub: [vinionix](https://github.com/vinionix)
- LinkedIn: [vfidelis](https://www.linkedin.com/in/vfidelis)
