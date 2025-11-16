# Python AI Coder - Assistente de Programação Python

### 📋 Descrição

O **AI Coder** é um assistente de IA especializado em programação Python, desenvolvido para ajudar desenvolvedores iniciantes com dúvidas de código através de uma interface web interativa.

### 🚀 Instalação e Configuração

### Pré-requisitos
- Python 3.13 (recomendado usar `mise` para controle de versão)
- Anaconda/Miniconda
- Chave de API da Groq

### Passos de Instalação

1. **Crie o ambiente virtual:**
   ```bash
   conda create --name ai-coder-env python=3.13
   ```
2. **Ative o ambiente:**
   ```bash
   conda activate ai-coder-env
   ```
3. **Instale as dependências:**
   ```bash
   conda install pip
   pip install -r requirements.txt
   ```
## 🎯 Como Usar

1. **Execute a aplicação:**
   ```bash
   streamlit run ai_assist.py
   ```
2. **Configure a API:**

- Insira sua API Key da Groq na barra lateral

- Obtenha uma chave em: https://console.groq.com/keys

3. Faça suas perguntas:

- Digite suas dúvidas sobre Python no campo de chat

- O assistente responderá com explicações, exemplos de código e referências

## 💡 Exemplos de Perguntas:
```bash
Como crio um hello world em Python?

Qual a sintaxe de um loop em Python?

Como eu uso a função map em Python? Me dê um exemplo com lambda.

Como trabalhar com list comprehension?

Qual a diferença entre listas e tuplas?
```

## 🏗️ Arquitetura do Sistema

### - Componentes Principais:

**ai_assist.py: Aplicação principal Streamlit**

**requirements.txt: Dependências do projeto**

**Groq API: Integração com modelo de linguagem**

### - Fluxo de Funcionamento

**Interface Streamlit captura pergunta do usuário**

**Sistema envia prompt para API Groq com regras específicas**

**IA processa e retorna resposta formatada**

**Resposta exibida com:**

- Explicação conceitual

- Exemplo de código comentado

- Detalhes da implementação

- Documentação de referência

### 📝 Estrutura das Respostas

- Todas as respostas seguem o formato:

```bash
text
📝 Explicação Clara
   → Explicação direta e didática do conceito

💻 Exemplo de Código
   → Código Python bem comentado

🔍 Detalhes do Código
   → Explicação linha por linha

📚 Documentação de Referência
   → Link para documentação oficial
⚙️ Configurações Técnicas
```

### Modelo:

- OpenAI GPT OSS 20B via Groq

- Temperature: 0.7 (balance entre criatividade e precisão)

- Max Tokens: 2048

- Foco Exclusivo: Programação Python

### 🛑 Encerrando o Ambiente

```bash
# Desativar ambiente
conda deactivate

# Remover ambiente (opcional)
conda remove --name ai-coder-env --all
```

### ⚠️ Observações Importantes

- O assistente foca exclusivamente em programação Python

- Sempre verifique as respostas - IA pode cometer erros

- Mantenha sua API Key segura

- Use para aprendizado e consulta, não para produção

