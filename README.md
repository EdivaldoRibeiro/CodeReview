# CodeReview
Meus aprendizados sobre `Code Review`

#### 1 - Projeto responsabilidade de todos os colaboradores.

- Análise minunciosa do código, buscando não apenas erros mas falhas que são exploradas por malévolos.
- Fechar portas abertas sem uso.
    
#### 2 - Todo o time responsável pelo projeto.

- Automatização de trabalhos manuais diminuem falhas humanas.
- Testes automáticos garantem que BUGs não serão implantados em novas e existentes implementações.
- Rastrear, discutir, resolver situações onde houver `code smell`.
    
#### 3 - Cada colaborador revisar a solução apresentada antes de integrá-lo ao código base.

- Compartilhamento de conhecimento.
- Criação de soluções alternativas para problemas.
- Aumento do senso da equipe.
- Confiança da equipe.
- Tirar responsabilidade de uma só pessoa, evitar filas com domínio individual.

#### 4 - Uso de container. (Mundo `docker`)

- Container específico para autenticação de usuários.
- Container específico para cada tipo de banco de dados.
- Container específico para cada webserver afim.
- Container específico para cada tipo de micro-serviço bem definido.
- Container específica para determinada regra de negócio.
- Desacoplar para ampliar a modularidade e melhorar o processo de testes.
- Garantir bom funcionamento na ligação de todos estas interfaces.
- Salvar imagens para posteriores instalações.

#### 5 - Padronização.
 
- Nos projetos JAVA adicionar plugin `checkStyle` garantindo que toda equipe respeitem o estilo adotado na organização.
- Nome **coerente** para classes, métodos e variáveis.
- Tamanho **limitado** de linhas dos métodos, dividir classe muito grande em classes menores.
- Métodos devem ter no máximo 3 parâmetros.
- Nunca manter código comentado que ficou em desuso.
- Desacoplar para ampliar a modularidade e melhorar o processo de testes.
- Executar um método Java num contexto transacional de banco de dados sem ter que conhecer ou manipular de forma alguma JTA;
- Executar um método Java local que acesse um remoto sem ter que conhecer ou manipular de forma alguma RMI, por exemplo;
- Utilizar-se de mecanismos de gerenciamento sem ter que conhecer ou manipular de forma alguma JMX;
- Tornar um método Java local em um handler de mensageria sem ter que conhecer ou manipular de forma alguma JMS;
- JavaConfig mecanismo que possibilita configurar diretamente nas classes java por meio de metadados na forma de annotations.

#### 6 - Ferramenta de análise. _SonarQube_

- O SonarQube é uma plataforma de código aberto desenvolvida pela SonarSource para inspeção contínua da qualidade do código para realizar revisões automáticas com análise estática de código para detectar bugs, códigos cheirosos e vulnerabilidades de segurança em mais de 20 idiomas de programação.
    
- Instalar Docker Container.
- Carregar imagem do SonarQube
    - docker pull sonarqube
    - Completar instalações.
- Configurar `maven` para alimentar banco de dados do **_SonarQube_**.

#### 7 - Suporte para novos projetos.

- O site 'http://www.setupmyproject.com' dá suporte para iniciar vários modelos de projetos Java.
- O site 'https://spring.io/guides' dá suporte para iniciar vários modelos de projetos usando Spring boot.

#### 8 - Meu container do postgresql.

-mkdir ~/postgresql
-cd ~/postresql
-docker pull centos/postgresql-96-centos7
-docker run -ti --name postgresql_database -e POSTGRESQL_USER=user -e POSTGRESQL_PASSWORD=pass -e POSTGRESQL_DATABASE=db -p 5432:5432 centos/postgresql-96-centos7
-netstat -anp |grep 5432
-dbeaver 5.2.5

