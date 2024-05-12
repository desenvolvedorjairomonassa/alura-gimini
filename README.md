# alura-gimini desafio

criar um projeto usando generativo AI da google, gimini.

<img src="work-dd0908f-2302-4c4f-87c9-d23630abcd54.jpg" alt="Descrição da imagem">


# 1. Motivação:

O mercado de trabalho brasileiro é complexo e as leis trabalhistas podem ser difíceis de entender, especialmente para quem não possui conhecimento jurídico. Isso pode gerar insegurança e frustração para os trabalhadores, que muitas vezes não sabem como defender seus direitos e muitas vezes nem sabem seus direitos

# 2. Ideia:

Criar um aplicativo de agente virtual que utilize inteligência artificial (IA) junto como modelos LLM para auxiliar trabalhadores com dúvidas sobre seus direitos trabalhistas. O aplicativo irá:

- **Responder perguntas frequentes**: O agente virtual será treinado com base na CLT e em outras leis trabalhistas, para que possa responder perguntas frequentes sobre diversos temas, como férias, horas extras, rescisão de contrato, entre outros.
- **Fornecer informações personalizadas**: O agente virtual também poderá fornecer informações personalizadas com base na situação específica do trabalhador. Para isso, o trabalhador poderá fornecer informações sobre seu caso, como tipo de contrato, cargo, tempo de serviço, etc.
- **Indicar um advogado**: Se o trabalhador precisar de um suporte mais especializado ou para com processo na justiça, o aplicativo poderá indicar um advogado mais perto de sua região. O aplicativo também poderá enviar ao advogado uma sumarização da --conversa entre o trabalhador e o agente virtual, com a autorização do mesmo.
- **Permitir o envio de dúvidas por texto ou voz**: O trabalhador poderá enviar suas dúvidas ao aplicativo por texto ou voz, de acordo com sua preferência.

  # 3.Arquitetura

  O aplicativo será desenvolvido utilizando a tecnologia Gemini, uma plataforma de IA da Google. O Gemini será utilizado para treinar o agente virtual com base na CLT e em outras leis trabalhistas. A CLT será vetorizada para que possa ser facilmente consultada pelo agente virtual. A consulta será feita por similaridade, o que significa que o agente virtual irá procurar por leis que sejam semelhantes à dúvida do trabalhador.
  
  A v1 pretendo usar somente o gimini, sem considerar fazer nenhum tunning e nem fazer nem um evaluation de modelo, a não ser uma validação manual, verificando se a resposta está de acordo. Fazendo os primeiros testes, ele começou a bloquear as respostas pois, as pessoas podem enviar "discurso de ódio", como por exemplo: "meu partão não me dá férias". Desenho da arquitetura 1:
  
<img src="Captura de tela 2024-05-11 222650.png" alt="Descrição da imagem">

  
  Já estou analisando em colocar um documento de clt para dar mais credibilidade trazendo grounding.

  Análise evolução da arquitetura:

  1 - Utilizando cloud run para criar o indíce e outro para fazer os RAG
  <img src="Captura de tela 2024-05-11 221723.png" alt="Descrição da imagem">
  

  # 4.Nome do aplicativo

   Justiça na mão ou Justiça na Palma da mão
  
  # 5. Nome do agente virtual

  Justino ou Justina
