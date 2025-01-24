# RAG_local_usando_Ollama

- Implementação baseada no artigo: [Build your own RAG and run it locally: Langchain + Ollama + Streamlit](https://medium.com/@vndee.huynh/build-your-own-rag-and-run-it-locally-langchain-ollama-streamlit-181d42805895)

Foi usado a plataforma Ollama que permite executar modelos de linguagem em computadores locais, utilizando tecnologia otimizada para rodar grandes modelos de IA de forma eficiente e privada. Seu objetivo é facilitar o uso de Large Language Models (LLMs) sem depender da nuvem, fornecendo maior controle sobre os dados e menor latência para aplicações locais. Pode se escolher entre diversos modelos, conforme [lista](https://ollama.com/search).

Para essa implementação foi usado o [modelo deepseek-r1](https://ollama.com/library/deepseek-r1:1.5b) de 1.5B, porém o modelo pode ser modificado de forma simples no código.
Para interface é usada a biblioteca [Streamlit](https://streamlit.io/) que é de código aberto em Python e facilita a criação de aplicativos web interativos.

Para esse experimento foi anexado documentos com informações controladas e depois feito perguntas diretamente no chat em linguagem natural em português. O resultado foi satisfatório, ainda mais usando o modelo mais básico com 1.5B de parâmetros. Novos testes alterando o template do prompt no código serão executados futuramente.

## Como rodar

- No terminal do computador digitar: ollama serve
- Em outro terminal do computador iniciar o modelo: ollama run deepseek-r1:1.5b
- Para rodar a aplicação: streamlit run app.py

Ao finalizar os testes dar um stop:

- no terminal do serve: ctrl+c
- do modelo: ollama stop deepseek-r1:1.5b
