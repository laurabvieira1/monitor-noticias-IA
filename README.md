# 📰 Monitor de Notícias sobre Inteligência Artificial

Automação desenvolvida com **n8n** para monitorar notícias relacionadas à Inteligência Artificial, utilizando feeds RSS para coletar, filtrar e organizar conteúdos relevantes, com envio automático das atualizações por e-mail.

## Objetivo

Facilitar o acompanhamento de notícias sobre Inteligência Artificial por meio de um processo automatizado de busca, filtragem e distribuição de informações, reduzindo a necessidade de pesquisas manuais.

## Tecnologias e ferramentas

- **n8n:** Plataforma utilizada para construir e executar o fluxo de automação.
- **RSS Read:** Coleta notícias por meio de feeds RSS.
- **Google News RSS:** Fonte de notícias sobre Inteligência Artificial.
- **JavaScript:** Tratamento e organização dos dados coletados.
- **Gmail:** Envio automático das notícias por e-mail.

## Como funciona

O fluxo é composto pelas seguintes etapas:

1. **Schedule Trigger:** Inicia a automação automaticamente no horário programado.
2. **RSS Read:** Consulta o feed RSS do Google Notícias utilizando o tema Inteligência Artificial.
3. **Filter:** Filtra as notícias de acordo com os termos configurados.
4. **Remove Duplicates:** Evita o processamento de notícias já identificadas em execuções anteriores.
5. **Code in JavaScript:** Organiza os títulos, datas e links das notícias em um formato HTML.
6. **Send a message (Gmail):** Envia um e-mail contendo as notícias encontradas.

## 🖥️ Fluxo da automação

![Fluxo completo da automação](docs/imagens/Fluxo.n8n.png)

## Evidências do projeto

### Execução do workflow

![Execução da automação](docs/imagens/Executado.png)

### Resultado do envio

![E-mail recebido](docs/imagens/Gmail.jpeg)

## Como executar

1. Instale ou acesse uma instância do n8n.
2. Importe o arquivo JSON disponível na pasta `workflow/`.
3. Configure uma credencial válida do Gmail.
4. Defina o endereço de e-mail destinatário.
5. Ative o workflow e configure o agendamento.

## Observações

Este projeto utiliza o Google Notícias por meio de RSS e foi desenvolvido para demonstrar a aplicação prática de automações na coleta e distribuição de informações sobre Inteligência Artificial.
O workflow disponibilizado neste repositório possui dados de identificação e credenciais removidos. É necessário configurar novamente a conexão com o Gmail antes da execução.

---

**Projeto desenvolvido para fins de aprendizado e portfólio.**
