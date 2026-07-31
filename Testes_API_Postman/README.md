# Como Utilizar o Postman para Testar API

[← Voltar](https://github.com/joycequoos/Test_QA/blob/main/README.md)

Guia com as funcionalidades mais básicas do Postman, aplicadas em um exemplo prático de teste de API.

## Sobre o Postman

O Postman é uma ferramenta gratuita amplamente utilizada para testar, desenvolver e documentar APIs. Ele permite enviar requisições HTTP (GET, POST, PUT, DELETE, entre outras) para um endpoint, visualizar a resposta retornada e validar se a API está se comportando conforme o esperado — sem a necessidade de escrever código para isso.

- **Organização por Workspaces** — permite separar os testes por projeto, mantendo coleções de requisições organizadas.
- **Interface intuitiva** — facilita a montagem de requisições, o envio de parâmetros e a análise das respostas da API.
- **Colaboração** — workspaces podem ser compartilhados entre equipes, facilitando o trabalho conjunto entre QA e desenvolvimento.
- **Amplamente usado em testes de API** — é uma das ferramentas mais adotadas por times de QA para validar o comportamento de APIs de forma rápida e visual.

## Configurando o Postman

### 1. Baixar o Postman

Acesse o site oficial do Postman e realize o download da ferramenta.

![Site Oficial - Download Postman](01_Site_Oficial_DownloadPostman.GIF)

### 2. Fazer Login no Postman

Após instalar, faça login na ferramenta.

![Logando no Postman](02_Logando_Postman.GIF)

### 3. Criar um Workspace por Projeto

O recomendado é criar um workspace específico para cada projeto, mantendo os testes organizados.

![Criando um Workspace](03_Workspace.GIF)

**Exemplo de workspace:**

![Exemplo de Workspace](04_Workspaces_Da_Aula.GIF)

### 4. Criando o Primeiro Workspace

Crie o seu primeiro workspace na ferramenta.

![Criando o Primeiro Workspace](05_MeuPrimeiroWorkspace.GIF)

### 5. Apresentação do Workspace

Visão geral da interface do workspace recém-criado.

![Apresentação do Workspace](06_Apr_Workspace.GIF)

## Opções para Testes

O Postman oferece diferentes formas de testar uma API. Entre as principais funcionalidades disponíveis na ferramenta:

![Funcionalidades do Postman](07_Funcoes.GIF)

### Utilizando o HTTP Request

Para testar uma API, a opção utilizada é o **HTTP Request**.

![HTTP Request](08_HTTP_Request.GIF)

## Testando uma API com o Método GET

### 1. Método GET

O método **GET** é utilizado para solicitar dados de um recurso específico, sem alterar nada no servidor.

![Método GET](09_Metodo_Get.GIF)

### 2. Comandos para Testar APIs

Principais comandos e campos utilizados na montagem de uma requisição de teste.

![Comandos para Testar APIs](10_Comandos_TestarAPIs.GIF)

### 3. API Utilizada no Exemplo

Para este exemplo, foi utilizada a API pública da Binance:

```
https://api.binance.com/api/v3/avgPrice?symbol=BTCUSD
```

![Link da API Utilizada](11_LinkAPIUtilizada.GIF)

### 4. Parâmetros

Os parâmetros da requisição (como o `symbol`) são configurados na aba correspondente do Postman.

![Parâmetros](12_Parametros.GIF)

### 5. Enviando e Verificando o Retorno da API

Após configurar a requisição, clique em **Send** para enviá-la e visualizar o retorno da API.

![Enviando a Requisição (Send)](13_SEND.GIF)

### 6. Resultado com Parâmetro Correto

Ao corrigir o parâmetro `symbol` para o valor esperado pela API, o retorno é validado com sucesso.

![Resultado com Parâmetro Correto](14_Resultado_Param_Correto.GIF)

**URL correta utilizada no exemplo:**

```
https://api.binance.com/api/v3/avgPrice?symbol=BTCUSDT
```

## Considerações Finais

Esse exemplo mostra na prática um erro comum em testes de API: um parâmetro incorreto (`BTCUSD` em vez de `BTCUSDT`) pode fazer a requisição falhar mesmo com toda a configuração correta. Por isso, validar cuidadosamente os parâmetros enviados é uma das etapas mais importantes ao testar uma API — e o Postman torna esse processo rápido e visual, sem a necessidade de escrever código.

## Conteúdo Relacionado

- [Test_QA — repositório principal](https://github.com/joycequoos/Test_QA)

