# Sistema de assinatura #

Sistema responsável por gerenciar, realizar a cobrança recorrente e cancelamento o de assinaturas do serviço VoxMe.

### Como realizar a instalação? ###

* Pré requisitos: Node.js.
* Clone o repositório.

```shell
$ git clone `https://youruser@bitbucket.org/askauxilium/vxm_ms_subscriptions.git`
```

* No diretório do projeto clonado execute o comando a seguir para instalar as dependências.

```shell
$ npm install
```

* Para verificar a cobertura dos testes unitários execute na parta da raiz do projeto e na pasta commons.
```shell
$ npm run coverage
```

* Para executar somente os testes unitários.
```shell
$ npm run test 
```

* O realizar o deploy para alpha o CI/CD irá automáticamente subir o serviço para a AWS.
* Na AWS poderão ser acessados os lambdas e os serviços de configuração, permissões e monitoramento.
* Configurações:
  * Nas configurações estão as variáveis de ambiente incluindo as configurações para acesso ao banco de dados.
  * No botão testar poderão ser usados os modelos de requests de cada lambda para testar o funcionamento do serviço.
* Monitoramento
  * É possível as métricas do lambda especifico e acessar os logs.
  * Os logs podem ser acessados pelo botão "Visualizar logs no CloudWatch"
  * Nos logs também é possível, caso necessário, verificar a resposta de um objeto especifico do código (usando console.log(obj)).
