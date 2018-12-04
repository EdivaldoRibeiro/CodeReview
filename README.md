# CodeReview
Meus aprendizados sobre "Code Review"

#### 1 - Projeto responsabilidade de todos os colaboradores.

- Análise minunciosa do código, buscando não apenas erros mas falhas que são exploradas por malévolos.
- Fechar portas abertas sem uso.
    
#### 2 - Todo o time responsável pelo projeto.

- Automatização de trabalhos manuais diminuem falhas humanas.
- Testes automáticos para garantir que BUGs não sejam implantados.
- Rastrear, discutir, resolver situações onde houver "code smell".
    
#### 3 - Cada colaborador revisar a solução apresentada antes de integrá-lo ao código base.

- Compartilhamento de conhecimento.
- Criação de soluções alternativas para problemas.
- Aumento do senso da equipe.
- Confiança da equipe.
- Tirar responsabilidade de uma só pessoa, evitar filas individuais de solução.
 
#### 4 - Padronização.
 
- Projeto JAVA adicionar plugin "checkStyle" garantindo que todo os envolvidos respeite estilo comun de organização.

#### 5 - Ferramenta de análise. _SonarQube_

- O SonarQube é uma plataforma de código aberto desenvolvida pela SonarSource para inspeção contínua da qualidade do código para realizar revisões automáticas com análise estática de código para detectar bugs, códigos cheirosos e vulnerabilidades de segurança em mais de 20 idiomas de programação.
    
- Instalar Docker Container.
- Carregar imagem do SonarQube
    - docker pull sonarqube
    - Completar instalações.
