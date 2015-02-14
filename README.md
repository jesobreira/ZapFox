[![Stories in Ready](https://badge.waffle.io/jesobreira/ZapFox.png?label=ready&title=Ready)](https://waffle.io/jesobreira/ZapFox)
## ZapFox — Cliente ZapZap para Firefox OS

Este aplicativo é um fork do [Telegram/Webogram](https://github.com/zhukov/webogram/) com estilo alterado para ser similar ao [ZapZap](http://zapzap.gratis).


### Interface


Aqui estão alguns screenshots do aplicativo:


![Adicionar novo contato](/app/img/screenshot/1.png)
![Informação do contato](/app/img/screenshot/2.png)
![Conversa](/app/img/screenshot/3.png)


### Ainda não suportado

* Chats secretos
* Lista negra
* Mensagens autodestrutivas
* ZapMapa (check-in)
* ZapGrupos
* ZapMural

Nota: esses 3 últimos encontram-se com problemas. Os mesmos já foram reportados à PrivateHost e o desenvolvimento ***não*** deve iniciar até que os mesmos sejam corrigidos.


### Maintained locations


| Descrição        | URL           | Tipo  |
| ------------- |-------------| -----:|
| Versão web online (hospedado no Meu ZapZap)      | http://meu.zapzap.gratis/ | hosted
| Versão web online (hospedado no Github Pages)      | https://jesobreira.github.io/ZapFox | hosted
| Firefox & FirefoxOS Marketplace | https://marketplace.firefox.com/app/zapfox |    packed



**Hosted**: o aplicativo é aberto como um website comum. Pode funcionar off-line devido ao cache.

**Packed**: o aplicativo é baixado para o dispositivo.

## Bugs

O projeto Webogram foi desenvolvido por [@zhukov](https://github.com/zhukov), então fique à vontade para relatar problemas relacionados com a funcionalidade do aplicativo [aqui](https://github.com/zhukov/webogram/issues). Bugs a respeito do visual do aplicativo podem ser reportados [aqui](https://github.com/jesobreira/ZapFox/issues).


## Detalhes técnicos

Este aplicativo faz uso do framework AngularJS, escrito puramente em Javascript. jQuery é utilizado para manipulações do DOM, e Bootstrap é o framework CSS.


#### Rodando localmente pelo servidor web

O webogram não faz uso de linguagens server-side. Desta forma, qualquer servidor web (Apache, nginx etc.) está habituado a rodá-lo. Se você não tiver um servidor web instalado, o repositório inclui um servidor bem simples, mas é suficiente para executar o prgorama.

Para rodar este servidor, instale o [node.js](http://nodejs.org/) e execute `node server.js`. Em seguida, abra http://localhost:81/app/index.html em seu navegador.

#### Rodando como uma extensão do Google Chrome

Para rodar essa aplicação no Google Chrome como uma extensão, abra essa URL no Chrome: `chrome://extensions/`. Após, clique em "Modo do desenvolvedor" > "Carregar extensão...". Selecione a pasta "app" do repositório e o ZapZap aparecerá na lista.

#### Rodando como aplicação Firefox OS

Para rodar essa aplicação no Firefox, pressione Alt, abra Menu > Desenvolvedor > WebIDE (ou pressione `Shift + F8`). Escolha "Abrir aplicativo empacotado" do menu Projeto e selecione a pasta "app" do repositório.

### Preparando para distribuição

O aplicativo, apesar de completamente funcional, é bloqueado em algumas plataformas, como o Firefox OS, devido às políticas de [CSP](https://developer.mozilla.org/pt-BR/Apps/CSP).

O repositório traz um diretório "dist", onde se encontra o aplicativo já compilado. Entretanto, as modificações deverão ser feitas no diretório "app" e, após tais modificações, o mesmo deverá ser compilado. Leia a página [Compilando](https://github.com/jesobreira/ZapFox/wiki/Compilando) na Wiki para obter instruções.


### Bibliotecas de terceiros

Além dos frameworks supracitados, outras bibliotecas foram usadas para suprir as necessidades do protocolo e da interface gráfica. Aqui estão algumas delas:

* [JSBN](http://www-cs-students.stanford.edu/~tjw/jsbn/)
* [CryptoJS](https://code.google.com/p/crypto-js/)
* [zlib.js](https://github.com/imaya/zlib.js)
* [UI Bootstrap](http://angular-ui.github.io/bootstrap/)
* [jQuery Emojiarea](https://github.com/diy/jquery-emojiarea)
* [nanoScrollerJS](https://github.com/jamesflorentino/nanoScrollerJS)
* [gemoji](https://github.com/github/gemoji)
* [emoji-data](https://github.com/iamcal/emoji-data)
 

Nossos sinceros agradecimentos a todos os autores e contribuintes dessas bibliotecas. A lista detalhada com descrições e licenças está disponível [aqui](/app/vendor).


### Licença

Este código está licenciado sob a licença GPL v3. A licença está disponível [aqui](/LICENSE).


### [Contribua](CONTRIBUTING.md)
