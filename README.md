# Como começar

A API Zoop está implementada em conformidade com o princípio de design [REST](https://en.wikipedia.org/wiki/Representational_state_transfer). Nossa API possui recursos orientados a URLs, com códigos HTTP para indicar erros. Nós utilizamos funcionalidades HTTP nativas, como verbos de ação POST, PUT, GET, DELETE, para operações de leitura e escrita, bem como o modelo [básico de autenticação](https://en.wikipedia.org/wiki/Basic_access_authentication) HTTP.

Nós suportamos chamadas diretas aos recursos da API a partir de outras origens, [CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing) \(cross-origin resource sharing\), permitindo você interagir de maneira segura com nossas APIs a partir de aplicações web, lembrando sempre de utilizar sua chave pública nesses casos, reservando sua chave secreta para chamadas internas de sistema. Todas as respostas da API estão no formato de dados JSON, incluindo errors.

Para permitir que você possa explorar todos os serviços sem preocupação, nossas contas possuem chaves de acesso nos modos de produção \(LIVE\) e teste \(TEST\). Não é possível alternar entre modos, basta usar a chave apropriada para realizar operações em produção ou ambiente de teste. Chamadas feitas com chaves de teste não são processadas junto a instituições bancárias, facilitando o desenvolvimento.

## Como organizamos a documentação?

### Marketplace

Nessa área concentramos todos os objetos bases para iniciar a integração. Como gestão de vendedores, compradores, documentos.

Saldo de conta e histórico de lançamentos.

Tokenização de cartões e contas bancárias.

Cadastro de usuários administrativos do marketplace.

Gestão de api keys.

{% page-ref page="api/marketplace/" %}

### Métodos de cobrança

A autorização em si.

{% page-ref page="api/metodos-de-cobranca.md" %}

### Pagamentos e transferências

Payout

{% page-ref page="api/pagamentos-e-transferencias.md" %}

### Planos e Assinaturas

subscriptions

{% page-ref page="api/planos-e-assinaturas.md" %}

### Notificações

webhooks

{% page-ref page="api/notificacoes.md" %}



