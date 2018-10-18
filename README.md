# Introdução

A API Zoop está implementada em conformidade com o princípio de design [REST](https://en.wikipedia.org/wiki/Representational_state_transfer). Nossa API possui recursos orientados a URLs, com códigos HTTP para indicar erros. Nós utilizamos funcionalidades HTTP nativas, como verbos de ação POST, PUT, GET, DELETE, para operações de leitura e escrita, bem como o modelo [básico de autenticação](https://en.wikipedia.org/wiki/Basic_access_authentication) HTTP.

Nós suportamos chamadas diretas aos recursos da API a partir de outras origens, [CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing) \(cross-origin resource sharing\), permitindo você interagir de maneira segura com nossas APIs a partir de aplicações web, lembrando sempre de utilizar sua chave pública nesses casos, reservando sua chave secreta para chamadas internas de sistema. Todas as respostas da API estão no formato de dados JSON, incluindo errors.

Para permitir que você possa explorar todos os serviços sem preocupação, nossas contas possuem chaves de acesso nos modos de produção \(LIVE\) e teste \(TEST\). Não é possível alternar entre modos, basta usar a chave apropriada para realizar operações em produção ou ambiente de teste. Chamadas feitas com chaves de teste não são processadas junto a instituições bancárias, facilitando o desenvolvimento.

Fique por dentro de todas as publicações e anúncios de APIs e SDKs da Zoop acessando nossa [lista de publicações](https://groups.google.com/a/pagzoop.com/forum/#!forum/zoop-api---publicaes).
