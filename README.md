# azure-ai-document-translator

-----

````markdown
# 🤖 Solução de Tradução Automática de Documentos Técnicos com Azure AI

## 📜 Descrição do Projeto

Este projeto implementa uma solução de **tradução automática** focada na precisão e contexto de artigos e documentação técnica. Utilizamos o **Azure Cognitive Services Translator** para processar documentos no formato `.docx` parágrafo por parágrafo, garantindo que a estrutura do documento original seja mantida e que a tradução seja salva em um novo arquivo.

O projeto foi desenvolvido como parte de um curso especializado para demonstrar proficiência em integração de serviços de IA em aplicações Full-Stack de nível Básico.

## ✨ Funcionalidades Principais

* **Processamento de Arquivos:** Leitura e escrita de documentos usando a biblioteca `python-docx`.
* **Integração com Azure AI:** Uso da API do Azure Translator para tradução robusta e escalável.
* **Manutenção de Estrutura:** O código itera sobre o documento, garantindo que apenas o texto seja traduzido, mantendo a formatação e quebras de linha.
* **Saída Padronizada:** O arquivo traduzido é salvo com um sufixo de idioma (`_pt-br.docx`).

## 🛠️ Tecnologias e Dependências

* **Linguagem:** Python 3.x
* **Serviço de IA:** Azure Cognitive Services Translator (API REST)
* **Bibliotecas Python:**
    * `requests` (Para comunicação com a API do Azure)
    * `python-docx` (Para manipulação de arquivos Word)

As dependências podem ser instaladas via `pip` usando o arquivo `requirements.txt`:
```bash
pip install -r requirements.txt
````

## 🚀 Configuração e Execução

### 1\. Obtenção de Credenciais

Este projeto requer acesso a um recurso **Azure Cognitive Services Translator**. As seguintes variáveis devem ser obtidas no painel "Keys and Endpoint" do seu recurso Azure:

  * **`subscription_key`:** chave secreta de acesso.
  * **`endpoint`:** URL base da API (ex: `https://api.cognitive.microsofttranslator.com/`).
  * **`location`:** Região onde seu recurso foi criado (ex: `eastus2`).

-----

## 📂 Estrutura do Repositório

```
azure-ai-document-translator/
├── README.md               <-- Este arquivo
├── requirements.txt        <-- Dependências Python
├── translate_solution.ipynb  <-- Código principal (Funções translate_document e translation_text)
├── docs/                   <-- Contém imagens, screenshots de configuração, etc.
│   └── azure_config.png
└── samples/                <-- Contém arquivos de entrada e saída para teste
    ├── musica_there.docx     <-- Documento original
    └── musica_there_pt-br.docx <-- Documento traduzido (Resultado)
```

```

---
