# Imersão IA Alura Google

# Chatbot com Detecção de Fake News

Este programa é um chatbot que utiliza o modelo Gemini Pro da Google para responder perguntas, mas com um diferencial: ele inclui um sistema de detecção de fake news.

## Como funciona?

O chatbot verifica se a pergunta do usuário contém palavras-chave comumente associadas a notícias falsas. Se a pergunta for identificada como potencialmente relacionada a fake news, o chatbot emite um alerta e fornece links para sites de verificação de fatos.

## Para que serve?

Este programa tem como objetivo:

* **Informar:** Fornecer respostas às perguntas dos usuários usando o poder do modelo Gemini Pro.
* **Alertar:** Conscientizar os usuários sobre a presença de fake news em diversos temas.
* **Incentivar a verificação:** Direcionar os usuários para fontes confiáveis de informação para que possam verificar a veracidade das informações.

## Uso:

**1.Instale o SDK do Google:**
```bash
pip install -q -U google-generativeai
```
**2. Defina sua chave de API da Google:**

Obtendo sua API KEY para o Google AI Studio:

*Para utilizar algumas funcionalidades do Google AI Studio, você precisará de uma API KEY. Siga os passos abaixo para gerar a sua:*

2.1 - Acesse o Google AI Studio: Vá para o site do Google AI Studio.

2.2 - Abra o menu lateral: Clique no ícone de três linhas 
horizontais no canto superior esquerdo da tela para abrir o menu lateral.

2.3 - Selecione "Get API Key": No menu lateral, localize e clique na opção "Get API Key".

2.4 - Copie a API KEY: Uma janela pop-up exibirá sua API KEY. Copie essa chave.

2.5 - Armazene sua API KEY: Guarde sua API KEY em um local seguro. Você poderá utilizá-la para autenticar suas requisições à API do Google AI Studio.

**Observações:**

Segurança da API KEY: Trate sua API KEY como uma senha. Não a compartilhe publicamente, em repositórios de código ou em outros locais inseguros.
Limitação de uso: O uso da API do Google AI Studio pode estar sujeito a limites e custos, dependendo do seu plano. Verifique a documentação oficial para obter mais informações.
Com sua API KEY em mãos, você poderá começar a utilizar os recursos avançados do Google AI Studio e integrar seus projetos a outros serviços.

**3. Acesse suas chaves de secret em Python:**

Para proteger informações sensíveis, como API Keys, tokens de acesso e credenciais, em seus projetos do Google Colab, utilize o recurso de "secrets" do Colab. Ele permite armazenar dados de forma segura, evitando a exposição direta no código.
Configurando seus Secrets:

3.1 - Abra o notebook do Colab: Acesse o notebook onde você deseja utilizar os secrets.

3.2 - Acesse o menu "Secrets": Clique em Edit > Notebook settings > Secrets.

3.3 - Adicione um novo secret: Clique em Add secret.
Defina nome e valor:

3.4 - Secret name: Escolha um nome descritivo para o seu secret (ex.:**SECRET_KEY**).

3.5 - Secret value: Insira o valor do seu secret.

3.6 - Salve o secret: Clique em Save secret.

Acessando seus Secrets no código:
Para acessar o valor de um secret em seu código:

```python
    from google.colab import userdata
    google_api_key = userdata.get("SECRET_KEY")
    genai.configure(api_key=google_api_key)
```

## Execute o programa:
**O chatbot iniciará uma conversa, aguardando sua pergunta.**

*Digite sua pergunta:*

**O chatbot responderá à sua pergunta, e caso o tema seja frequentemente associado a fake news, ele exibirá um alerta e links para sites de verificação.**

*Digite "fim" para encerrar a conversa.*

**Observações:**

A lista de palavras-chave e sites de verificação de fatos pode ser atualizada para abranger novos temas e fontes de informação.
Este programa é um exemplo básico e pode ser expandido para incluir funcionalidades adicionais, como a verificação de fatos em tempo real utilizando APIs de checagem.

## Referência

 - [Alura](https://www.alura.com.br/)
 - [Imersão IA Alura+Google](https://www.alura.com.br/imersao-ia-google-gemini)
 - [Google Gemini](https://gemini.google.com/app)
 - [Google AI Studio](https://aistudio.google.com/app/prompts/new_chat)


## Autores

Este programa foi desenvolvido durante as aulas da imersão. Este programa foi modificado acrescentando a funcionalidade de detecção de risco de fake news através do uso do Google Gemini, e do Google AI Studio, usando os métodos ensinados de como criar prompts no Google IA Studio para criação de código e a integração ao código existente.

