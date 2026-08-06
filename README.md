# From Zero to MiniGPT

Construindo modelos de Inteligência Artificial do zero, desde os fundamentos matemáticos até um pequeno modelo de linguagem baseado na arquitetura Transformer.

O objetivo deste repositório não é apenas utilizar bibliotecas prontas ou consumir APIs de modelos existentes. A proposta é compreender, implementar, testar e documentar os principais componentes envolvidos na construção de modelos modernos de IA.

## Objetivo

Responder, na prática, à seguinte pergunta:

> Como um modelo de Inteligência Artificial aprende e como podemos construir um pequeno modelo de linguagem compreendendo cada uma de suas partes?

O projeto combina quatro frentes em cada etapa:

1. **Matemática:** compreender e derivar as equações principais.
2. **Implementação:** transformar os conceitos em código, começando com Python e NumPy.
3. **Experimentação:** modificar parâmetros, provocar falhas e medir o comportamento.
4. **Documentação:** registrar resultados, limitações, erros e aprendizados.

## Roadmap

- [ ] Fundamentos matemáticos computacionais
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

## Estrutura planejada

```text
from-zero-to-minigpt/
├── 00_project_foundations/
├── 01_math_foundations/
├── 02_linear_regression/
├── 03_logistic_neuron/
├── 04_mlp_backpropagation/
├── 05_sequence_models/
├── 06_embeddings/
├── 07_self_attention/
├── 08_transformer/
├── 09_minigpt/
├── 10_post_training/
├── 11_llm_system/
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

### Etapas avançadas

- PyTorch
- FastAPI
- Docker
- Modelos abertos e bibliotecas de tokenização
- Bancos vetoriais
- Ferramentas de avaliação de LLMs

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

## Autor

Desenvolvido por Vinícius Fidelis.

- GitHub: [vinionix](https://github.com/vinionix)
- LinkedIn: [vfidelis](https://www.linkedin.com/in/vfidelis)
