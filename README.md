# Apenas alguns codigos que fiz para estudos

Este repositório reúne implementações simples e diretas em Python (Jupyter Notebooks) para demonstração e testes de diversas ferramentas de Inteligência Artificial. O foco aqui é cobrir desde o consumo de APIs comerciais modernas até a execução local de modelos de NLP e geração de imagens.

## Estrutura do Repositório

###  01 API LLM
Centraliza os scripts de integração com as principais APIs de modelos de linguagem (LLMs) do mercado para tarefas de chat e completude de texto.
* **`GPT.ipynb`**: Integração com a API da OpenAI utilizando o modelo `gpt-3.5-turbo`.
* **`gemini.ipynb`**: Implementação utilizando a biblioteca oficial do Google (`google-generativeai`) com o modelo `gemini-1.5-pro`.
* **`deepseek.ipynb`**: Exemplos de consumo da API do DeepSeek de duas formas diferentes: utilizando o SDK da OpenAI (com `base_url`) e fazendo requisições HTTP diretas via biblioteca `requests`.

---

###  02 modelos Transformers
Dedicado ao uso da biblioteca `transformers` da Hugging Face para tarefas clássicas de Processamento de Linguagem Natural (NLP), rodando os modelos localmente.
* **`gerar_textos.ipynb`**: Geração de texto contínuo utilizando uma versão em português do GPT-2 (`pierreguillou/gpt2-small-portuguese`).
* **`sumarizar_textos.ipynb`**: Sumarização automática de textos longos utilizando a arquitetura T5 multilíngue (`csebuetnlp/mT5_multilingual_XLSum`).
* **`completar_textos.ipynb`**: Previsão de palavras ocultas (estilo teclado inteligente) baseado em técnica de *Masked Language Modeling* com o BERT adaptado para o português (`neuralmind/bert-base-portuguese-cased`).

---

### 03 Geração de imagens
Focado na geração de conteúdo visual a partir de prompts textuais (*Text-to-Image*), abordando tanto soluções proprietárias via nuvem quanto open-source locais.
* **`dalle.ipynb`**: Geração de imagens utilizando o modelo `dalle-3` da OpenAI via API, convertendo a URL de resposta em exibição direta no notebook.
* **`stablediffusion.ipynb`**: Pipeline local utilizando a biblioteca `diffusers` para carregar e rodar o modelo de código aberto `StableDiffusionXLPipeline` com suporte a aceleração por GPU (CUDA).

---
