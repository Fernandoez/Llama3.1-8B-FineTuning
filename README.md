# Fine-Tuning de LLM para Geração de Questões de Programação

Este repositório contém o notebook utilizado para o projeto final da disciplina **Processamento de Linguagem Natural**, ministrada no **Programa de Pós-Graduação em Ciência da Computação (PPGCC) da Universidade Federal de Ouro Preto (UFOP)**.

## Objetivo

Demonstrar a eficácia do fine-tuning de um modelo LLM (Llama 3.1-8B), mesmo com uma quantidade pequena de questões incialmente (10), para gerar automaticamente questões práticas de programação em português, seguindo uma estrutura padronizada.

## Principais Características

- **Modelo usado**: Llama 3.1-8B via [Unsloth](https://github.com/unslothai/unsloth).
- **Técnicas aplicadas**: QLoRA, PEFT (LoRA).
- **Tarefa**: Geração de enunciados de questões com tema e tópico definidos (foco em decisão simples em Python).
- **Formato de dados**: Alpaca prompt (instruction, input, output) e questões formatadas em LaTeX.
- **Ambiente de execução**: Google Colab (GPU T4).

## Resultados

- Modelo fine-tunado obteve **80% de acurácia** ao gerar questões seguindo o padrão definido.
- Modelo zero-shot (sem ajuste fino) falhou em todos os casos testados. O modelo seguia para uma reposta direta com código, sem seguir o tópico solicitado e sem gerar enunciado. 

## Conteúdo

- `notebook.ipynb`: código completo para fine-tuning e geração.
- Questões usadas para treinamento, estruturadas e com prompts correspondentes.
