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



## 3. Primeiros passos para desenvolvimento Web

 ### Início da internet:

1969 - USA

1989 - USA uso comercial

1992 - WWW (World Wide web)

Brasil - 1994 - uso comercial Embratel - conexão discada

​             2000 - banda larga

### Termos chave

HTML - linguagem de marcação (não é linguagem de programação)

HTTP - protocolo de internet

Link - ligação

URL - endereço (ex.: quando colocamos uma URL no whatsapp, ele já cria um link)

Pixel - picture elements

Span - lixo eletrônico

Virus - Software malicioso

Keylogger - captura tudo o que é digitado

phishing - intenção de roubar enganando outras pessoas (ex.: "sites similares")

Firewall - impedir acesso indevido

Clickbait

Facke news - boatos da internet (click dá dinheiro)

Podcast - programas de rádio

### Protocolos de comunicação

TCP / IP - Transmition Control Protocol / Internet Protocol

**Modelo de camadas:** 

4 camadas: 	

1. Física (ex.: placa de rede ou wi-fi)

      2. Rede (ex.: IP)
         3. Transporte (ex.: TCP, UDP)
           4. Aplicação (ex.: FTP (arquivos), SMTP (e-mails), HTTP (internet))

**UDP x TCP**:

**UDP:** Rápido, não confiável, carro do ovo, usado para Livestream (só dispara)

**TCP:** Voltado à conexão, handshake, integridade, ordem dos dados, usado para aplicatido de mensagens de texto (mantém tudo organizado)

### Portas

São as "portinhas" por onde os dados sirão e chegarão

- 20 FTP - arquivos
- 22 SSH - conexão pura entre computadores
- 25 SMTP - e-mails
- 53 DNS - Domain Name Service - endereço
- 80 HTTP internet
- 443 HTTPS internet

### Modem, Roteador e Switch

**Modem:**

Combinação de: Modulator / Demodulator

Hardware que converte dados em formato que possa ser transmitido.

**Roteador:**

Distribui internet para um ou mais dispositivos de rede

Pode ser burro (transmite tudo para todos)

**Switch:**

Criado para ser inteligente (transmite só para quem pediu, o que foi pedido)

### Dados Móveis

SMS (texto)

MMS (aúdio e vídeo)

Conexões móveis  (Wi - Fi)( 3G - 7Mbps, 4G - 22,1Mbps, 5G - 10 Gbps)

Segurança: 

WEP: chaves de 64 bits e de 128 bits

WPA: chaves trocadas periodicamente

WPA2: (AES) (802.11i) , mais segurança, mais processamento (pode ser um pouco mais lento, mas quase imperceptível)

#### Bluetooth

Conexão ponto a ponto (não precisa de rede/internet)

### Browser / Navegador

Interpreta LP (Linguagem de Programação) em algo compreensível para o humano.

É possível acessar a internet sem um navegador (ex.: comandos - FTP)

Mas acessar os sites, só por meio de um navegador.

#### Cache:

Partes dos sites gravados no computador (para carregar mais rápido)

#### Cookies:

Rastro que os sites deixam no computador / dispositivo e as redes sociais e criadores de anúncios usam para mostrar anúncios personalizados.

#### Site:

Página da internet, diversos propósitos, diversas LP, D/XHTML caindo em desuso.

#### Aplicativo:

Um software que é executado no navegador, muitas vezes é uma espécie de navegador, hoje em dia quase não existe diferença entre site e aplicativo. 

Outra diferença terminológica que está sumindo é entre programa / software / aplicativo.

#### E-commerce:

Comércio eletrônico.

Site com sistema de pagamento. O sistema de pagamento pode ser exterior ao site: ex.: picpay, boleto, pagseguro, mercado pago, etc.

#### Web Server:

Onde ficcam guardados os softwares, sites.

**Estático:** é um servidor físico onde são armazenados arquivos, softwares, banco de dados.

**Dinâmico:** se refere aos softwares que estão presentes no servidor físico

- Arquivos (file server)
- Aplicações (application server)
- Banco de dados (database)
- Tudo junto e misturado

#### Web Service:

Interface disponível para fazer requisições e consultas em bancos de dados inacessíveis. Correios, Governo.

#### Stacks:

- Pilhas de tecnologia
- Conjunto de softwares necessários e suficientes para executar um aplicativo / programa.
- Linguagens de Programação
- Ambientes e ferramentas de interação com app/sw.
- Capacidade e limitações de performance
- Pontos fortes e fracos do app/sw

É o ambiente tecnológico todo da empresa.

**Importância:**

- Estratégias de negócios
- Maturidade
- Contratações, planos de mitigação de riscos, aumento da capacidade, uso de dados.

#### Front-end:

- Parte da frente, é o que você vê (ex.: site, word, etc.)
- Site, software, aplicativo, web service
- interface UI (user interface) / UX (user experience)
- Lógica de programação, HTML, CSS, jQuery, JS/AJAX, PHP, Bootstrap, Outros frameworks.

#### Back-end:

- Parte de trás
- Servidores, bancos de dados
- "meios-de-campo" entre interface e bancos de dados, regras de negócios, validações
- MySQL, Oracle, protocolos de comunicação, PHP, Java, node.js.

#### Full stack:

- Profissional que trabalha em todas as camadas das tecnologias de desenvolvimento.


#### LPs e Termos

**Principais Linguagens:**

- HTML - marcação
- CSS - marcação e estilo (mais opções que HTML)
- JavaScript (mais usada) (jQuery, AJAX, diversas libs)
- PHP - maipulação de dados
- .Net
- ASP
- Java - mais antiga
- Ruby (on Rails)
- Python
- Perl
- C / C++ / C# (mais baixo nível que as outras)

**Termos comuns:**

- 404 - Erro - página não existe
- Algoritmo - Sequência de passos para execução de uma tarefa.
- ALT - indexação
-  API - parte do site para usar em outro lugar
- Aplicação
- Back-end
- Biblioteca / dll
- Bootstrap
- Break points - pontos chaves para diversos dispositivos (debug - parada)
- Browser / navegador
- Bug
- Cache
- Código - instruções para que um aplicativo ou site seja executado
- Controle de versão
- Cookies
- Debug
- Design adaptativo / responsivo
- Deploy  - pacotinho para ser publicado
- DNS - Domain Name Service
- Documentação: interna (comentários no programa) / externa (manual do usuário)
-  Domínio: .com / .com.br
- DPI - proporção de pontos na tela.
- Editor de texto
- Estrutura de dados - fila, pilha, array
- Faricon - figurinha que define o site
- Fontes
- Framework - caixa de ferramentas disponíveis
- Front-end
- FTP - protocolo de transmissão de arquivos
- Full stack
- GitHub / SVN / CVS - controladores de versão
- HTTP(s) - protocolo de comunicação
- IP - protocolo de internet (número de identificação)
- Linguagem
- Meta tags
- Método ágil
- Mobile
- MVC - model view controler
- MVP - minimo produto viável
- MySQL
- Pixel - pix + element
- Resolução - quantidade de pixels na tela
- Servidor
-  Sistema Operacional - Windows, Linux, etc
- Solução - um programa ou um conjunto de programas para solucionar um problema
- SSL - segurança
- UI - user interface
- UX - user experience
- Versão (ex.: maiores 1.0 para 2.0 e menores 2.0 para 2.1)
- WYS/WYG - What you see - What you get






