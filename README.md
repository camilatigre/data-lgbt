# LGBT Youtube Content Analysis
### O objetivo é entender alguns comportamentos relacionados ao uso de hashtags da comunidade lgbtqiap+ e o que isso pode significar quanto ao conteúdo postado no YouTube para esse público.

### **Onde conseguir dados?**
O primeiro desafio consiste em ter dados relacionados ao uso de hashtags que indicam conteúdo relacionado à essa comunidade. Algumas hashtags consideradas nesses dados:	
	
- queer, lgbt, lesbian, bisexual, pansexual, gay, trans, nonbinary, intersex, asexual

Esses dados serão extraídos por uma ferramenta chamada [Octoparse](octoparse.com/) que devolverá uma lista de vídeos com as hashtags listadas e criará uma tabela com os seguintes dados:

- Id, video_title, video_link, channel_name, channel_link, total_views, publish_data, description
	

### **Formatação, normalização e padronização dos dados**
Nessa etapa será feita uma análise para remoção de linhas duplicadas, remoção de nulos e vazios. Também irá ser criada uma nova variável(coluna) a partir de alguma informação que temos e também uma para guardar o dia da semana relacionado a data de publicação. Ficando assim com esse resultado:
	
- Id, video_title, video_link, channel_name, channel_link, total_views, publish_data, description, tags, publish_day

Ações:
- [ ] Padronização de tempo de publicação para meses
- [ ] Criação de uma coluna "Taxa de crescimento diário médio". 
	- Fórmula: Taxa de visualizações diárias = Total de visualizações / Tempo decorrido desde a publicação
- [ ] Criar coluna de "Dia da semana publicação" para descobrir qual era o dia da semana naquela data de públicação

### Algumas perguntas para serem analisadas
- [ ] Os vídeos com maior visualização foram postados em quais dias da semana?
- [ ] A média de visualização por canal tem correlação com os termos utilizados?
- [ ] Qual é a duração dos vídeos mais visualizados?
- [ ] Qual é a duração dos vídeos mais visualizados?
- [ ] Quais as tags **mais** utilizadas em vídeos de maior visualização?
- [ ] Quais as tags **menos** utilizadas em vídeos de maior visualização?

### Hipoteses
1. Existe relação entre a duração do vídeo e o crescimento em visualizações de vídeo. -[ ] Verdadeiro - [ ] False
2. Existe relação entre as tags utilizadas e o crescimento em visualizações de vídeo. -[ ] Verdadeiro - [ ] False
3. Existe relação entre o dia da semana postado e o crescimento em visualizações de vídeo. -[ ] Verdadeiro - [ ] False
