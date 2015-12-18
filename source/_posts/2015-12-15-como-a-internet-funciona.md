title: Como a internet funciona?
tags: 'internet, web'
date: 2015-12-15 00:07:50
---

![Internet - Rede Mundial de Computadores](http://placehold.it/1000x300?text=Rede Mundial)

Você sabe o que é a Internet? Como ela funciona? E a Web? Conhece?

Se você está lendo isso aqui, provavelmente você deve utilizar muito a internet.
A maioria das pessoas que a utilizam não fazem nem ideia de como ela funciona.
É como a energia elétrica em suas casas, todos sabem que é só ligar alguma coisa na tomada e pronto, vai funcionar.
Mas de onde vem essa energia? Como ela chega em minha casa? Bem, a internet é quase parecida com isso.

<!-- more -->

Para muitos, a primeira imagem que vem na cabeça ao pensar em Internet é esta:

![Nuvem](http://placehold.it/300x150?text=Nuvem)

Mesmo que hoje em dia fala-se muito de *Cloud Computing*, na verdade, ela não se parece em nada com isso.
A internet tem mais essa cara aqui:

![Cabo de Internet](http://placehold.it/300x150?text=Cabo de Rede)

Isso mesmo. Um cabo, ou um fio.

A internet ganha toda sua força porque através desse cabo, dois ou mais computadores podem ser ligados e trocar informações entre si.
Isso é a internet, uma rede mundial de computadores interligados que se comunicam através de alguns protocolos, que são como acordos ou contratos que definem como a comunicação será regida.
Para ser um pouco mais correto, a internet é uma rede várias outras redes constituída por empresas privadas, públicas, acadêmicas e de governo.

## A história

A origem da internet data da década de 60. Surgiu a partir de pesquisas militares durante a Guerra Fria.
Nessa época duas grandes potencias, União Soviética e Estados Unidos, exerciam grande influência no mundo através de seus blocos ideológicos e politicamente antagônicos.

Os Estados Unidos temiam um ataque, e qualquer inovação era bem vinda para proteger informações sigilosas a não serem trazidas a público. Então eles idealizaram um modelo de troca e compatilhamento de informações
que permitia a descentralização da informação. Assim se uma base militar fosse atingida as informações não seriam perdidas.
Assim nasceu a ARPANET, criada pela *Advanced Research Projects Agency* (ARPA).

O ataque inimigo da União Soviética, teóricamente, nunca existiu. Mas o que o Departamento de Defesa dos Estados Unidos não imagiva era que acabara de criar o maior fenômeno midiático do século 20.
Um sistema de comunicação capaz de atingir cerca de 50 milhões de pessoas em 4 anos.

Na década de 70 a tensão entre URSS e EUA diminuiu. Então o governo dos EUA permitiu os pesquisadores acadêmicos a utilizarem a ARPANET para que desenvolvessem suas pesquisas em suas respectivas universidades.
Com o crescente número de universidades utilizando a rede, o governo decidiu dividir o sistema em dois grupos: MILNET que possuia localidades militares, e a nova ARPANET com localidades não militares, que permitiu o desenvolvimento mais livre da rede, inclusive com a ajuda dos alunos.

A partir daí a INTERNET foi surgindo e se desenvolvendo. Jovens da [contracultura](https://pt.wikipedia.org/wiki/Contracultura) movidos por uma *utopia* de difusão da informação tiveram um papel muito influente na criação dessa rede.
O governo dos Estados Unidos novamente investiu na internet, patrocinando o desenvolvimento de Backbones, que são como grandes computadores que tem uma capacidade poderosa de dar vazão a uma grande quantidade de fluxo de dados, como canais de fibra ótica, elos de satélite, ou elos de transmissão via rádio.

Seja por interesses acadêmicos, militares, ou visando o grande potencial financeiro e rentável daquela novidade, a internet recebeu ajuda/influência de pesquisadores universitários como do MIT, de empresas privadas como a IBM, de políticos como o senador norte-americano Al Gore e também de estudantes.

Bom, concluindo, a internet é uma grande infraestrutura de rede de computadores.
Porém o termo Internet e Web são frequentemente usados como sinônimos. É bastante comum ouvir alguém falar "navegar na internet".
Enquanto a internet é a rede, a Web é apenas um dos muitos serviços que funcionam através da internet.
A Web é uma aplicação. Uma coleção de documentos (páginas web) e outros recursos como imagens, vídeos ou documentos pdf ligados por *hiperlinks* e URLs e acessados/consumidos por um programa de computador chamado *navegador*.
Além da Web existem outros serviços/aplicações que funcionam através da internet como e-mails, transferencia de arquivos, controle remoto de computador, jogos e etc.
A Web (World Wide Web ou WWW) foi criada em 1992 pelo cientista Tim Berners-Lee, do CERN (Organização Europeia para a Investigação Nuclear).

## Ok, Ok. Chega de História. Como tudo isso realmente funciona?

Bem, vamos lá.

Imagine que você mora na casa de número **187.10.145.12** e na sua casa tem várias portas, uma delas é a porta **64001**.
E você quer pedir um pouco de açucar para o seu amigo que mora na casa **173.194.118.33** e você vai bater na porta **80**.
Se você precisa pedir açucar para o seu amigo, primeiro você precisa saber onde ele mora. E depois você precisa bater em alguma porta para chamá-lo.

Com a internet é bem assim. Cada computador, celular, impressora ou qualquer outro dispositivo, ao se conectar numa rede como a internet recebe um endereço único, o IP.
Além desse IP, seu computador possui muitas portas por onde ele pode se comunicar com outro computador.
Então se o seu computador quer acessar e consumir o conteúdo do Google, por exemplo, ele precisa saber primeiro qual é o IP do Google e qual porta ele deve bater para pedir a informação.

Essa comunicação entre o seu computador, que está consumindo a informação, e o outro computador que possui a informação a ser consumida, é chamada de arquitetura Cliente Servidor.
Onde Cliente é o seu computador, e Servidor é o computador que fornece a informação.

![Cliente Servidor](http://placehold.it/300x150?text=Cliente Servidor)

Ok, mas como eu vou saber qual é o IP e a porta do Google? Eu só digito www.google.com.br na barra do navegador e já funciona!

## DNS - Domain Name System

DNS, ou sistema de nomes de domínios, são como listas telefônicas. Todo computador ao ligar na internet está configurado a acessar um DNS.

Então quando você digita www.google.com.br no seu navegador, você está informando a ele a URL (Uniform Resource Locator) do web site que você quer acessar, neste caso o Google.

Então o seu navegador tenta lembrar se ele já conhece o endereço IP desse tal de Google, assim como você já sabe onde seu amigo do açucar mora pois você já precisou dele várias vezes, certo?

Caso o seu navegador ainda não conheça o endereço do Google, ele se conecta ao DNS - Telefonista ;) - e pergunta qual o endereço do Google.

> \- Olá, boa tarde. Eu gostaria de saber o endereço desse cara aqui: www.google.com.br
> \- Pois não, aguarda só um momentinho que estarei verificando senhor.
> \- [...]
> \- [...] 
> \- [...] (alguns milisegundos depois)
> \- Senhor, encontrei o endereço. Anota aí: **173.194.118.33**
> \- Ok, obrigado.
> \- ~~O senhor pode aguardar e avaliar meu atendimento?~~ (Mentira)

Bom, já temos o endereço IP do Google, mas e a porta?

Bem, na verdade você não precisa saber qual a porta da casa do seu amigo para você ir lá, certo?
Afinal você já sabe em qual porta bater. A que está de frente pra rua, certo?
A não ser que você seja muito amigo, você não vai entrar numa propriedade privada, escolher qual porta bater e pensar: huum, acho que vou bater nessa porta dos fundos.
Você faria isso caso você tivesse uma permissão expressa do seu amigo, dizendo: Ei, da próxima vez entre pela porta da cozinha.

Bem, na internet é mais ou menos isso. As portas são conhecidas.
Se você quer acessar uma página web, você vai bater na `porta 80`. Para transferir um arquivo, utilize a `porta 21`.
Para acessar um e-mail é `porta 25`, mas se você for um cara VIP, você pode talvez utilizar a `porta 587`.

## TCP/IP - Os Correios da Internet

Uma vez que os endereços são conhecidos, é preciso enviar a informação com o pedido/requisição e receber a resposta.
Mas como funciona essa troca de informação?

> \- Olá amigo **173.194.118.33**, posso me conectar pela porta **80**?
> \- Fala aí **187.10.145.12**, claro que pode. Inicie a conexão.
> \- Ok, vou começar a conexao então.
> Os pacotes começam a ser enviados...

Bem, a responsabilidade de como essa conexão deve funcionar é dada ao *Protocolo TCP* (Protocolo de controle de transmissão). Ele define como a informação deve ser trafegada de forma confiável.
A informação é quebrada em vários pacotes e ele possui mecanismos para verificar se o pacote foi recebido ou não para que esses possam ser montados no destino, caso tenham saído de ordem durante o trânsito.
Ele não se preocupa com o que está sendo transferido. Apenas tenta garantir que as informações cheguem ao seu destino corretamente.

Algumas características básicas dessa comunicação são:
* É uma comunicação de duas vias. O cliente fala com o servidor e o inverso é verdadeiro.
* Garantia de entrega, o que é enviado chegará ao destino corretamente. Na ordem correta e sem violações. É como se fosse uma carta registrada dos Correios.
* Controle de Fluxo, a quantidade de pacotes enviados aumenta ou diminui conforme a necessidade e a capacidade do destinatário.

Ok, existe uma comunicação estabelecida, dados estão sendo trafegados pelo TCP.
Mas como acontece a mágica da Web? Como o servidor sabe qual página quero ver?
Como ocorre a comunicação do meu navegador com o servidor?

## O Protocolo HTTP

O protocolo HTTP (Hypertext Transfer Protocol) é quem define como vai funcionar a comunicação da aplicação web. Para que o HTTP possa transferir suas informações pela web, é necessário que os protocolos TCP e IP tornem possível a conexão entre clientes e servidor, levando e trazendo os pacotes. Lembra dos Correios?

O HTTP possui algumas características básicas:
* Utiliza o modelo cliente-servidor, ou seja, o cliente requisita um documento e o servidor responde ou não com o documento solicitado.
> Cliente: \- Mãe, o que vai ter para o almoço?
> Servidor: \- Arroz, feijão e ovo.
* Ele é *stateless*, ou seja, não guarda informações de requisições anteriores. É como se ele tivesse problemas de memória.
> Cliente: \- Mãe, o que vai ter para o almoço?
> Servidor: \- Arroz, feijão e ovo.
> Cliente: \- Já está pronto?
> Servidor: \- Oi? Hein? Não entendi.

    Com isso, ele não é capaz de reter informações entre as requisições. Para isso você deve utilizar [cookies](https://pt.wikipedia.org/wiki/Cookie_HTTP), [sessões](https://pt.wikipedia.org/wiki/Sess%C3%A3o_%28ci%C3%AAncia_da_computa%C3%A7%C3%A3o%29), campos de formulário ou variáveis na própria url.

    > Cliente: \- Mãe, o que vai ter para o almoço?
    > Servidor: \- Arroz, feijão e ovo.
    > Cliente: \- Mãe, o almoço com arroz, feijão e ovo já está pronto?
    > Servidor: \- Está quase pronto.

Essa comunicação cliente-servidor é feita através de mensagens. O cliente envia uma mensagem de requisição, e o servidor retorna uma mensagem de resposta. Essas mensagens são compostas por um formato específico. É como um acordo de um idioma próprio. Esse idioma/acordo é definido pelo [RFC](https://www.ietf.org/rfc/rfc2616.txt).

Cada mensagem, seja de requisição ou resposta, possui uma linha inicial, nenhuma ou mais linhas de cabeçalho onde são informadas as opções, tipos e outras configurações necessárias. Obviamente também temos o corpo da mensagem que é opcional em determinados casos.

Exemplo de uma requisição, onde é solicitada a página web.
```
GET / HTTP/1.1
Host: www.google.com.br
User-Agent: Mozilla/5.0 (Windows NT 6.2; WOW64; rv:42.0) Gecko/20100101 Firefox/42.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: pt-BR,pt;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
Connection: keep-alive
```

Exemplo de resposta de uma página web.
```
HTTP/1.x 200 OK
Date: Fri, 04 May 2007 16:05:43 GMT
Server: Apache/2.0.59 (Unix) mod_ssl/2.0.59 OpenSSL/0.9.7a DAV/2 PHP/4.4.4 mod_bwlimited/1.4
Cache-Control: no-cache
Keep-Alive: timeout=3, max=100
Connection: Keep-Alive
Transfer-Encoding: chunked
Content-Type: text/html; charset=iso-8859-1

<html></html>
```

Hoje o HTTP está presente em muito de nossas vidas. Outras aplicações além do seu navegador ou de servidores web sabe falar e interpretar esse "idioma". Desde ferramentas de linha de comando, sua smart tv, até seu smartphone sabem lidar com esse protocolo.

Este é um diagrama que mostra o passo a passo de como a internet funciona:

![Diagrama de Sequencia - Cliente Servidor](http://placehold.it/800x500?text=Diagrama de Sequencia - Cliente Servidor)

É claro, existe muitos outros detalhes mais técnicos por traz dessa maravilha chamada internet.
Mas isso que tentei demonstrar é o básico para quem deseja trabalhar nessa área de desenvolvimento web.

A compreensão desde conteúdo inicial ajudará no entendimento de outros conceitos mais relacionados ao desenvolvimento web. **Bons estudos!**