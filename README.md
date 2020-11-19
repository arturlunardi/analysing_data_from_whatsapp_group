# Analisando os dados de um grupo de WhatsApp

Este repositório foi inspirado no post [Analisando os dados das mensagens de WhatsApp do meu relacionamento](https://medium.com/@hugotrigueiro/analisando-os-dados-das-mensagens-de-whatsapp-do-meu-relacionamento-fad214f8e4e4).

## Estrutura do projeto:

## 1. Coleta de dados

Para realizar a coleta dos dados, foi necessário [exportar a conversa de um grupo do WhatsApp](https://faq.whatsapp.com/android/chats/how-to-save-your-chat-history/?lang=pt_br). Os dados são exportados em formato txt. As mensagens foram exportadas sem mídias, dessa maneira as mensagens que possuiam mídias são transformadas em texto para que possam ser identificadas.

## 2. Tratamento e processamento dos dados

Como o formato do arquivo é txt, precisamos realizar uma série de processamentos e tratamentos para adequa-los e armazena-los em um dataframe.
As mensagens possuem o formato: **[dd/mm/yyyy hh:mm:ss] Autor: Mensagem**
Dessa maneira, utilizamos algumas técnicas para separar cada tipo de informação. Foram também criadas colunas extras para realizar a contagem de cada tipo de texto, como emojis, links, figurinhas etc.
Para realizar uma análise temporal, foram criadas séries temporais com as datas.

## 3. Análise dos dados

A análise dos dados foi basicamente divida em duas partes:
- Análise de texto

Nessa etapa foram utilizadas técnicas para descobrir quais eram os padrões de mensagens, quais emojis eram mais utilizados, quem eram as pessoas mais ativas do grupo, quais palavras são mais utilizadas etc.
- Análise gráfica

Na análise gráfica utilizamos de gráficos para visualizar as informações, utilizando bastante da análise de texto previamente realizada e também visualizando os padrões de acordo com as séries temporais criadas.

## 4. Conclusões

Foi possível identificar através desse projeto:
- Pessoas mais ativas no grupo
- Meses e dias da semana em que o grupo é mais ativo
- Palavras mais utilizadas pelos integrantes
- Como o grupo se comporta de acordo com o horário do dia
- Comportamento da atividade do grupo de acordo com as séries temporais
- Quantidade de mensagens, caracteres, figurinhas, emojis, links, mídias do grupo

E para você, o que mais podemos descobrir analisando um grupo de WhatsApp?

Contato:
[Linkedin](https://www.linkedin.com/in/artur-lunardi-di-fante-393611194/)
