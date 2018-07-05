# TRABALHO 01:  Projeto Smart Villam
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Leonardo:leorfb3@gmail.com<br>
Rafael:xemrafinha0800@gmail.com<br>
...

### 2.INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados "Smart Villam"
<br>e motivação da escolha realizada. <br>
  
> O projeto "Smart Villam" tem o como sua finalidade, aprimorar e reduzir o custo de produções agrícolas em pequena e larga escala. Sabendo-se que grande parte do consumo da água do nosso planeta é oriundo das produções agrícolas e que diversas áreas do Brasil vêm passando por intensos períodos de seca, tivemos a ideia de desenvolver um sistema que consiga diminuir o desperdício nas plantações. O Projeto "Smart Villam" tem como objetivo aumentar a produtividade e diminuir o consumo de água nas fazendas através de um sistema inteligente que trabalha com o clima e com a umidade.
 

### 3.MINI-MUNDO Novo<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas) <br>
Entrevista com o usuário e identificação dos requisitos.<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processa r, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

> O Sistema "SmartVillam" conterá as informacões aqui detalhadas. Nas Estufas , serão instalados sensores em cada área de plantação. O usuário envia as informações sobre cada área de plantação, solo, cultura e nutrientes para o nosso banco de dados com as especificações do tamanho da área em hectares, a data em que a cultura foi plantada, as datas de fertilização,o tipo do solo da área, a média de litros d'água por dia, os nutrientes presentes no solo e suas quantidades, o tipo de cultura plantada, os períodos de colheita, a média de litros d'água por dia necessários, os nutrientes necessários para a plantação e sua quantidade, os tipos de nutrientes que serão relacionados com a necessidade da cultura e com o que o solo possui. Dos sensores são armazenados: Dados do clima local (temperatura e umidade relativa do ar), incidência luminosa, temperatura umidade e nutrientes do solo. Após analisar o ambiente, e com base nas informações das plantações enviadas pelo cliente, o SmartVillam executará a configuração específica da estufa para aquela plantação e enviará o feedback ao usuário informando sobre o estado do solo ( umidade, necessidade de fertilizantes, temperatura, etc). Após a configuração da estufa ser concluída, o sistema dá início ao processo de irrigação e controle do ambiente, o sistema usará os sensores novamente para analisar os fatores atuais do ambiente comparando com as primeiras amostragens para se readaptar às mudanças do ambiente. Quando a plantação estiver preparada para a colheita, com base nas informações coletadas ao longo do período, o sistema informará o usuário pelo aplicativo, onde o usuário pode acompanhar o processo à distância e fazer o que for preciso para manter as áreas sob controle.  

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser desenvolvidas. O princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas e/ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/discipbd1/trab01/blob/master/balsamiq.png?raw=true "Title")
![Arquivo PDF do Protótipo Balsamiq feito para o Projeto Smart Villam](https://github.com/SmartVillam/trabalho01/blob/master/arquivos/ProjetoSmartVillam.pdf)


#### 4.1 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
![Arquivo PDF da tabela de dados feita para o Projeto Smart Villam](https://github.com/SmartVillam/trabalho01/blob/master/arquivos/Tabela_de_dados_SmartVillam.xlsx)
    
#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informações?
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto
    
  O sistema SmartVillam envia os seguintes tipos de relatório de acordo com a demanda do usuário:
      -Relatório contendo as principais informações do usuário: Nome, e-mail, telefone e código;
      -Relatório contendo todas as áreas cadastradas pelo usuário;
      -Relatório contendo todas as informações básicas de uma certa área;
      -Relatório contendo as informações da cultura de uma área;
      -Relatório contendo as informações do solo de uma área;
      -Relatório contendo a diferença de nutrientes solo-cultura;
        
        
>## Marco de Entrega 01 em: (24/03/2018)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 5 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
    
    B) NOTACAO UML (Caso esteja fazendo a disciplina de analise)
    
    C) QUALIDADE 
        Garantir que a semântica dos atributos seja clara no esquema
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas    
        
![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/Conceitual_SmartVillam.png?raw=true "Modelo Conceitual")
    
   
    
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]
## Marco de Entrega 01 em: (20/04/2018)<br>
#### 5.2 DECISÕES DE PROJETO
    [atributo]: [descrição da decisão]
    
    EXEMPLO:
    a) Campo endereço: em nosso projeto optamos por um campo multivalorado e composto, pois a empresa 
    pode possuir para cada departamento mais de uma localização... 
    b) justifique!
    No sistema em geral, preferimos direcionar o foco das plantações, que antes eram fazendas e grandes plantações, para estufas com áreas de monocultura definidas pelo usuário, o que nos deu uma direção e um objetivo mais claros para trabalharmos;
    
    Nos campos de medidas (quantidades e tamanhos) por hora, optamos por utilizar o formato inteiro, para facilitar a manipulação dos dados.

#### 5.3 DESCRIÇÃO DOS DADOS 
    [objeto]: [descrição do objeto]
    
    USUARIO: Tabela que armazena as informações relativas ao usuario.
    NOME: Campo que armazena o nome de cada usuario da SmartVillam.
    SENHA: Campo que armazena a senha de cada usuario da SmartVillam. 
    CODIGO_USUARIO: Campo que armazena o codigo de usuario de cada usuario da SmartVillam.
    TELEFONE: Campo que armazena o telefone de cada usuario da SmartVillam.
    
    REGISTRO_AREA: Tabela que armazena as informações relativas ao registro de áreas.
    NUMERO_DE_AREA: Campo que armazena o numero da área registrada.
    CODIGO_USUARIO: Campo que armazena o codigo do usuario que registrou a área
    
    AREA: Tabela que armazena as informações relativas à área de cultivo.
    NUMERO_DE_AREA: Campo que armazena o numero de cada área da SmartVillam.
    TAMANHO: Campo que armazena o tamanho de cada área da SmartVillam.
    DATA_PLANTACAO: Campo que armazena a data em que se deu inicio a prantação em cada área da SmartVillam.
    CODIGO_DATA_FERTILIZACAO: Campo que armazena o codigo das datas de fertilização de cada área da SmartVillam.
    CODIGO_SOLO: Campo que armazena o codigo de solo de cada área da SmartVillam.
    CODIGO_CULTURA: Campo que armazena o codigo de cultura de cada área da SmartVillam.
    
    DATA_FERTILIZACAO: Tabela que armazena as informações relativas à data de fetilização da área.
    CODIGO_DATA_DE_FERTILIZACAO: Campo que armazena o codigo de cada data em que a área foi fertilizada
    DATA: Campo que armazena a data em que cada área foi fertilzada
    
    CULTURA: Tabela que armazena as informações relativas à cultura plantada.
    NOME: Campo que armazena o nome de cada cultura da SmartVillam.
    CODIGO_CULTURA: Campo que armazena o codigo de cada cultura da SmartVillam.
    CODIGO_PERIODO_DE_COLHEITA: Campo que armazena o codigo do periodo de colheita de cada cultura da SmartVillam.
    MEDIA_DE_AGUA_DIARIA: Campo que armazena a media de àgua diara necesasria para cada cultura da SmartVillam.
    
    PERIODO_DE_COLHEITA: Tabela que armazena as informações relativas ao periodo de colheita da cultura.
    CODIGO_DE_PERIODO: Campo que armazena o codigo de cada periodo de colheita.
    PERIODO_DA_COLHEITA: Campo que armazena o periodo de cada colheita.
    
    NECESSIDADE_NUTRIENTES: Tabela que armazena as informações relativas à necessidade de nutrientes da cultura.
    CODIGO_CULTURA: Campo que armazena o codigo de uma cultura que necessita de um nutriente.
    CODIGO_NUTRIENTES: Campo que armazena o codigo de um nutriente que é necessario para uma cultura.
    QUANTIDADE: Campo que armazena a quantidade necessaria de um nutriente para uma cultura.
    
    SOLO: Tabela que armazena as informações relativas ao solo de cultivo.
    NOME: Campo que armazena o nome para cada solo da SmartVillam.
    CODIGO_SOLO: Campo que armazena o codigo de cada solo da SmartVillam.
    MEDIA_AGUA_DIARIA: Campo que armazena a quantidade de água posta diariamente em cada solo da SmartVillam.
    
    POSSE_NUTRIENTES: Tabela que armazena as informações relativas à posse de nutriente do solo
    CODIGO_SOLO: Campo que armazena o codigo de um solo que possui um nutriente.
    CODIGO_NUTRIENTES: Campo que armazena o codigo de um nutriente presente em um solo.
    QUANTIDADE: Campo que armazena a quantidade de um nutriente presente em um solo.
    
    NUTRIENTE: Tabela que armazena as informações relativas ao nutriente.
    NOME: Campo que armazena o nome de cada nutriente da SmartVillam.
    CODIGO_NUTRIENTE: Campo que armazena o codigo de cada nutriente da SmartVillam.

>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6	MODELO LÓGICO<br>
        a) inclusão do modelo lógico do banco de dados
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)
        
![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/SmartVillam_Logico_1.png?raw=true "Modelo Lógico")


### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas DDL 
        (criação de tabelas, alterações, etc..)  

![Modelo Físico](https://github.com/SmartVillam/trabalho01/blob/master/arquivos/SmartVillam_Modelo_Fisico.txt?raw=true "Modelo Físico")

        
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físic
        b) formato .SQL
![Inserção de Dados](https://raw.githubusercontent.com/SmartVillam/trabalho01/master/arquivos/topico_8.1.txt "Inserção de Dados")


#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
![Criação de tabelas + Inserção de Dados](https://raw.githubusercontent.com/SmartVillam/trabalho01/master/arquivos/topico_8.2.txt "Criação de Tabelas + Inserção de Dados")

        
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
![Criação e  exclusão de tabelas + Inserção de Dados](https://raw.githubusercontent.com/SmartVillam/trabalho01/master/arquivos/topico%208.3.txt "Criação e Exclusão de tabelas + Inserção de Dados")


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

SELECT nome, senha, cod_usuario, email, telefone FROM usuario;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_usuario.png?raw=true "Title")

SELECT * FROM area_2;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_area_2.png?raw=true "Title")


SELECT * FROM registro;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_registro.png?raw=true "Title")


SELECT nome, cod_plant, fk_periodo_de_colheita_cod_pr_colh__pk, media_agua_diaria FROM cultura;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_cultura.png?raw=true "Title")


SELECT nome, cod_nutri FROM nutrientes;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_nutrientes.png?raw=true "Title")


SELECT * FROM data_fertilizacao;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_data_fertilizacao.png?raw=true "Title")


SELECT * FROM periodo_de_colheita;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_periodo_colheita.png?raw=true "Title")


SELECT * FROM possui;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_possui.png?raw=true "Title")


SELECT * FROM necessita;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_necessita.png?raw=true "Title")


SELECT nome, cod_solo, media_agua_diaria FROM solo;

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/tabela_solo.png?raw=true "Title")



#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

select nome, media_agua_diaria FROM solo
where media_agua_diaria > 2;


![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/consulta3.png?raw=true "Title")


select nome,cod_usuario as codigo, email, telefone from usuario
where cod_usuario < 2018000;


![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/consulta4.png?raw=true "Title")




#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
    
    
#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.
    
    
select nome,telefone from usuario
where telefone like '99%';

![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/consulta1.png?raw=true "Title")


select nome, fk_periodo_de_colheita_cod_pr_colh__pk, media_agua_diaria FROM cultura
where nome like '%o%';


![Alt text](https://github.com/SmartVillam/trabalho01/blob/master/imagens/consulta2.png?raw=true "Title")



#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>


#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        

## Marco de Entrega 02 em: (16/06/2018)<br>
### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (30/06/2018)
<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

#### 9.11	LISTA DE CODIGOS DAS FUNÇÕES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>


#### 9.12	GERACAO DE DADOS (MÍNIMO DE 100 MIL REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 100 mil registros
        b) tabelas diretamente relacionadas a tabela principal 10 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        

#### 9.13	Backup do Banco de Dados<br>
        Detalhamento do backup.
        a) Tempo
        b) Tamanho
        c) Teste de restauração (backup)
        d) Tempo para restauração
        e) Teste de restauração (script sql)
        f) Tempo para restauração (script sql)
<br>

Data de Entrega: (Data a ser definida)
<br>

#### 9.14	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
    a) Lista de índices, tipos de índices com explicação de porque foram implementados nas consultas 
    b) Performance esperada VS Resultados obtidos
    c) Tabela de resultados comparando velocidades antes e depois da aplicação dos índices (constando velocidade esperada com planejamento, sem indice e com índice Vs velocidade de execucao real com índice e sem índice).
    d) Escolher as consultas mais complexas para serem analisadas (consultas com menos de 2 joins não serão aceitas)
    e) As imagens do Explain devem ser inclusas no trabalho, bem como explicações sobre os resultados obtidos.
    f) Inclusão de tabela mostrando as 10 execuções, excluindo-se o maior e menor tempos para cada consulta e 
    obtendo-se a media dos outros valores como resultado médio final.
<br>
    Data de Entrega: (Data a ser definida)
<br>   

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.

    
### 12	TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>
        a) Outros grupos deverão ser capazes de restaurar o banco 
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho 
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho

### 13	DIFICULDADES ENCONTRADAS PELO GRUPO<br>  

    
>## Marco de Entrega 04/Entrega Final em: (Data definida no cronograma)<br>

       
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
   
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/

#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


        
        


    





