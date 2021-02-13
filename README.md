pandoc --number-sections -t html | pandoc -f html -t markdown

# PW-Lab1

**OBJECTIVO**: Nesta ficha criará uma página na Web e disponibilizá-la-á num servidor na nuvem, numa conta criada por si, analisando alguns aspetos.

**PRÉ-REQUISITOS**: Instale o VS Code para editar o código HTML. 

# 1. ALOJAMENTO DE PÁGINA NA CLOUD

## CRIAÇÃO DE UMA PÁGINA WEB
Crie uma pasta lab1. Dentro dessa pasta, crie o ficheiro index.html com o seguinte código fonte HTML.

![](index.png)

Crie, na pasta lab1, a pasta img, e guarde dentro desta a imagem  wordcloud.png.

![](wordcloud.png)

Abra o ficheiro index.html com um Browser para ver se visualiza a imagem em baixo.

## CRIAÇÃO DE REPOSITÓRIO GITHUB
Crie um repositório no GitHub, e faça push dos conteúdos da pasta lab1.

## ALOJAMENTO NO HEROKU
Crie uma conta no Heroku. Sincronize o GitHub com o Heroku, de forma a colocar disponível a página na cloud. Visualize a sua página no URL disponibilizado.


# 2. CONHECER A INTERNET

Vamos entender o modelo cliente-servidor da Internet. O browser do seu computador é o cliente, que faz pedido da página ao servidor Heroku onde está a sua página.

## Endereços IP
* Anote qual o endereço IP do seu computador. Pode obter isso de várias formas. A mais simples é perguntar no Google "what is my ip".
* Anote qual o endereço IP do seu telemóvel.
* Anote onde está localizado, usando por exemplo a ferramenta https://whatismyipaddress.com/ip-lookup
* Anote qual o endereço IP da máquina onde está alojada a sua página no Heroku, e onde este está localizado.


## Percurso
Traceroute (comando tracert) é uma ferramenta de diagnóstico que rastreia a rota que um pacote faz desde o seu computador até ao endereço IP destino. Este identifica os routers pelos quais esse pacote passa até o seu destino, indicando o tempo que demorou a chegar là. 

Abra a linha de comando e escreva tracert e especifique o endereço IP obtido anteriormente:
``> traceroute <endereço IP ou URL sua app>``
Usando o website https://db-ip.com/, anote os tuplos (cidade,pais) por onde o pacote passou para chegar ao seu destino. 

Explore também a ferramenta http://en.dnstools.ch/visual-traceroute.html, onde pode ver gráficamente a rota, a partir da Suíça. 


# 2. ACESSO HTTP A UMA PÁGINA WEB

## HTTP
Web browsers (clientes HTTP) sãplicações que enviam pedidos HTTP a um servidor e recebem uma resposta (arquitetura cliente-servidor). Tipicamente, corresponde ao cliente que navega e pede páginas com conteúdos ao servidor, e recebe e processa as respostas. Existem muitos navegadores tais como Chrome, Firefox, Safari. Recebem ficheiros em formato HTML que conseguem representar visualmente nuam interface gráfica de visualização.

No Chrome, abra a sua página Heroku. Visualise o código fonte, clicando com o botão direito do rato, e selecionando "ver código fonte" (view page source). Verifique, corresponde ao que escreveu!

## Inspect

Nessa mesma página faça agora inspect (botão direito do rato). Selecione a barra network. Clique num hyperlink do site. Explique o que aparece?

Identifique quantos ficheiros são descarregados na sequencia de um clique num hiperlink.
Identifique o tipo de ficheiros.
Identifique os timings deespera e de descarga.
Faça o mesmo para o sitewww.ubi.pt





Abra a página, e clique no botão direito e selecione Inspect, ou selecione Ctrl+Shift+i.
Explore os vários tabs em cima e tente entender o que estes indicam.

