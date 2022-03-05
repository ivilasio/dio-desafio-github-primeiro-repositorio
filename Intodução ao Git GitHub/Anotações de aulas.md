# Anotações de aulas da Dio

## 1. Estrutura de dados

Organizam os dados na memória do computador ou qualquer dispositivo de armazenamento de dados.

**Algoritmo**: é um conjunto de instruções estruturadas e ordenadas para realizar uma tarefa ou operação específica. Manipular dados (inserir, excluir, ordenar e processar)

**Principais estruturas:**

**Vetores e Matrizes:** todos os dados são do mesmo tipo.

**Registro:** os dados podem ser de tipos diferentes.

**Lista: ** Ligada ou duplamente ligada.

**Pilha:**  segue o FIFO / PEPS ou  o LIFO / UEPS

**Fila:** segue o FIFO / PEPS

**Árvore:** hierarquia / raiz

**Tabela Hash:** chaves associadas aos valores

**Grafos:** vértices / relacionamentos - objetos (vértices) e relacionamentos (arestas). Andar para todos os lados.  

## 2. Introdução ao Git e ao GitHub

**Git e GitHub** não são a mesma coisa, são tecnologias complementares

**Git** gerencia versão de códigos

**GitHub** armazena e distribui as versões

Link para download do Git: https://git-scm.com/download/win
O Git Bash é um terminal extendido para otimizar o uso do Git..

Git e GitHub utilizam o SHA1 para encriptação dos arquivos (40 dígitos ou caracteres).

SHA1 é uma forma curta de representar um arquivo.

#### Objetos fundamentais do Git:

**BLOBS**:  Contém metadados (BLOB, "\0", tamanho do arquivo e o conteúdo)  

**TREES** : Armazenam BLOBs. São responsáveis por montar a estrutura dos dados. Armazenam tamém o nome do arquivo. Apontam para BLOBs e/ou para outras Trees. 

**COMMITS**: Armazenam também o autor do arquivo. É o objeto que vai juntar tudo. 
É o objeto mais importante.
É uma forma segura de demonstrar que os arquivos não foram alterados.
Se alterar um arquivo, altera toda a estrutura: BLOB, TREE e COMMIT.

#### Comandos ####

**Git init** -Inicia o Git. Cria um repositório dentro da pasta

**Git add** - Coloca o arquivo na área de "Stage"

**Git commit** - Disponibiliza o arquivo no repositório

####Ambientes

**Ambiente de desenvolvimento**  - fica na máquina local.  Contém o *working directory*, a *Staging area* e o repositório local

Ao criar ou alterar um arquivo no *working directory*, precisa depois colocá-lo na *Staging área*. Para isso no *Git Bash*,  dar o comando: **git add * **(ou nome do arquivo), e em seguida passar para o repositório local através do comando: **git commit -m "breve descrição"**

Para passar para o repositório remoto (no GitHub), dar o comando: **git push origin master** e para passar o arquivo do repositório remoto para o local: **git pull origin master** ou **git clone < url>**

**Repositório remoto** - fica no servidor (nuvem) onde pode ser distribuído. Outros desenvolvedores podem contribuir. 

