=== Virtuaria - Jamef para Woocommerce ===
Contributors: tecnologiavirtuaria
Tags: shipping, shipping method, jamef, woocommerce
Requires at least: 4.7
Tested up to: 6.0.1
Stable tag: 1.0
Requires PHP: 7.3
License: GPLv3 or later
License URI: https://www.gnu.org/licenses/gpl-3.0.html

Adiciona a Jamef como método de entrega para o Woocommerce.

== Description ==

Utilize os métodos de entrega e serviços da Jamef com a sua loja WooCommerce.

Jamef é um método de entrega brasileiro.

Serviços:
 * Rodoviário;
 * Aéreo.

Este plugin foi desenvolvido sem nenhum incentivo da Jamef. Nenhum dos desenvolvedores deste plugin possuem vínculos com esta empresa. E note que este plugin foi feito baseado na documentação do Web Services Jamef.

**Observação:** Os prints foram feitos em um painel wordpress/woocommerce personalizado pela Virtuaria objetivando otimizar o uso em lojas virtuais, por isso o fundo verde.

**Para mais informações, acesse** [virtuaria.com.br - desenvolvimento de plugins, criação e hospedagem de lojas virtuais](https://virtuaria.com.br/).

= Compatibilidade =

Compatível com Woocommerce 5.8.0 ou superior

### Descrição em Inglês: ###

Use Jamef's delivery methods and services with your WooCommerce store.

Jamef is a Brazilian delivery method.

This plugin was developed without any input from Jamef. None of the developers of this plugin have ties to this company. And note that this plugin was made based on the Jamef Web Services documentation.


== Installation ==

= Instalação do plugin: =

* Envie os arquivos do plugin para a pasta wp-content/plugins, ou instale usando o instalador de plugins do WordPress.
* Ative o plugin.
* Navegue para Woocommerce -> Configurações -> Entrega > Áreas de entrega, escolha um área e adicione a “Jamef” e preencha as configurações.

= Requerimentos: =

1- Conta na [Jamef](https://jamef.com.br/);
2 - Ter instalado o [WooCommerce](http://wordpress.org/plugins/woocommerce/).

= Configurações do Plugin: =

1 - Com o plugin instalado acesse o admin do WordPress e entre em "WooCommerce" > "Configurações" > "Entrega" > "Áreas de entrega" > edite uma área de entrega adicionado o Jamef .
2 - Preencha os dados:
* CNPJ/CPF;
* Município de origem;
* Estado de origem;
* Tipo de produto;
* Filial de coleta;
* Usuário do portal jamef;
* Ambiente (produção ou sandbox).

Pronto, sua loja já poderá fazer cotações com a Jamef.

### Instalação e configuração em Inglês: ###

* Upload plugin files to your plugins folder, or install using WordPress built-in Add New Plugin installer;
* Activate the plugin;
* Navigate to WooCommerce -> Settings -> Shipping > Shipping Zone, choose Jamef and setup options.


== Frequently Asked Questions ==

= Qual é a licença do plugin? =

Este plugin está licenciado como GPLv3.

= O que eu preciso para utilizar este plugin? =

* Ter instalado uma versão atual do plugin WooCommerce.
* Possuir uma conta na Jamef.

= Quais são os métodos de entrega que o plugin aceita? =

São aceitos os seguintes métodos de entrega nacionais:
* Rodoviário;
* Aéreo.

= Onde configuro os métodos de entrega? =

Os métodos de entrega devem ser configurados em “WooCommerce” > “Configurações” > “Entrega” > “Áreas de entrega”.

Para a entrega nacional, é necessário criar uma área de entrega para o Brasil ou para determinados estados brasileiros e atribuir os métodos de entrega.

= Tem calculadora de frete na página do produto? =

Não, mas, está prevista a adição deste recurso.

= Este plugin faz alterações na calculadora de frete na página do carrinho ou na de finalização? =

Não, nenhuma alteração é feita, este plugin funciona esperando o WooCommerce verificar pelos valores de entrega, então é feita uma conexão com os Correios e os valores retornados são passados de volta para o WooCommerce apresentar.

Note que não damos suporte para qualquer tipo de personalização na calculadora, simplesmente porque não faz parte do escopo do plugin, caso você queira mudar algo como aparece, deve procurar ajuda com o WooCommerce e não com este plugin.

= Como resolver o erro “Não existe nenhum método de entrega disponível. Por favor, certifique-se de que o seu endereço está correto ou entre em contato conosco caso você precise de ajuda.”? =

Esta é uma mensagem padrão do WooCommerce que é exibida quando não é encontrado nenhum método de entrega.

Mesmo você configurando os métodos de entrega, eles não são exibidos quando a Jamef retorna mensagens de erro, por exemplo quando a região onde o cliente está não é coberta ou quando o peso do pacote passa do limite suportado.

Entretanto, boa parte das vezes esse tipo de coisa acontece porque os métodos e/ou produtos não foram configurados corretamente.

Aqui uma lista de erros mais comuns:

* Faltando CEP de origem nos métodos configurados.
* CEP de origem inválido.
* Produtos cadastrados sem peso e dimensões
* Peso e dimensões cadastrados de forma incorreta (por exemplo configurando como 1000kg, pensando que seria 1000g, então verifique as configurações de medidas em WooCommerce > Configurações > Produtos).
* E não se esqueça de verificar o erro ativando a opção de Log de depuração nas configurações de cada método de entrega. Imediatamente após ativar o log, basta tentar cotar o frete novamente, fazendo assim o log ser gerado. Você pode acessar todos os logs indo em “WooCommerce” > “Status do sistema” > “Logs”.
* Servidor estar com pouca memória.

= Erro 401 =
Este erro diz respeito à autenticação do acesso aos servidores da Jamef. Verifique o ambiente selecionado na configuração e se o mesmo está disponível para sua conta na Jamef.

== Screenshots ==

1. Configurações do plugin;
2. Cotação no carrinho de compras;
3. Cotação no checkout;
4. Edição do pedido.


== Upgrade Notice ==
Nenhuma atualização disponível

== Changelog ==
= 1.0.1 2023-05-08 =
* Correção de erro ao utilizar o plugin com debug desativado.
= 1.0 2022-10-13 =
* Versão inicial.