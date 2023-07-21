# LGBT Sentimental Analysis
### O objetivo é entender alguns comportamentos relacionados ao uso de hashtags da comunidade lgbtqiap+ e o que isso pode significar quanto ao conteúdo postado no YouTube para esse público.

### **Onde conseguir dados?**
O primeiro desafio consiste em ter dados relacionados ao uso de hashtags que indicam conteúdo relacionado à essa comunidade. Algumas hashtags consideradas nesses dados:	
	
- queer, lgbt, lesbian, bisexual, pansexual, gay, trans, nonbinary, intersex, asexual

Esses dados serão extraídos por uma ferramenta chamada [Octoparse](octoparse.com/) que devolverá uma lista de vídeos com as hashtags listadas e criará uma tabela com os seguintes dados:

- Id, video_title, video_link, channel_name, channel_link, total_views, publish_data, description
	

### **Formatação, normalização e padronização dos dados**
Nessa etapa será feita uma análise para remoção de linhas duplicadas, remoção de nulos e vazios. Também irá ser criada uma nova variável(coluna) a partir de alguma informação que temos. Ficando assim com esse resultado:
	- Id, video_title, video_link, channel_name, channel_link, total_views, publish_data, description, tags

Ações:
- [ ] Padronização de tempo de publicação para meses
- [ ] Criação de uma coluna "Taxa de crescimento diário médio". 
	- Fórmula: Taxa de visualizações diárias = Total de visualizações / Tempo decorrido desde a publicação
- [ ] Criar coluna de "Dia da semana publicação" para descobrir qual era o dia da semana naquela data de públicação

### Algumas Hipoteses para serem analisadas
- [ ] Qual é a relação entre o número de visualizações e a data de publicação dos vídeos? Existe alguma tendência de crescimento ou declínio ao longo do tempo?
- [ ] Exista alguma correlação entre o número de visualizações e o titulo do video? O que preciso para fazer essa análise?
- [ ] Os vídeos com maior visualização foram postados em quais dias da semana? Tem correlação?
- [ ] A média de visualização por canal tem correlação com os termos utilizados?
- [ ] Os vídeos com maior visualização e menor visualização. Quais são eles e quais os termos utilizados?
- [ ] Existe alguma correlação entre o número de visualizações e a duração dos vídeos?
