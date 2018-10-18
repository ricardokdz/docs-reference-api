# Autenticação básica

Nossas APIs REST permitem autenticação por token. Apenas um administrador de conta pode acessar ou gerar tokens de API.  
Quando sua conta está ativada para usar a API, a chave aparecerá na sua área de administrador no link OPÇÕES na seção PE.

A autenticação na API ocorre via autenticação de acesso básico HTTP. Você encontrará mais detalhes sobre Autenticação básica no IETF RFC 2617.

Forneça a sua chave como nome de usuário para a autenticação básica. Você não precisa fornecer uma senha.

Toda a comunicação deve ser criptografada via SSL. O token de autenticação básica é reversível, no entanto, como toda a comunicação é por HTTPS, o contexto de segurança está completamente protegido. Um aplicativo deve enviar um cabeçalho de Autorização HTTP contendo o nome de usuário a cada solicitação.

Todas as chamadas na API devem ser feitas por HTTPS para garantir a segurança.

Toda requisição recebida que não esteja criptografada será considerada comprometida pelo nosso sistema e irá falhar.

A autenticação básica é trivial para usar nas bibliotecas de clients HTTP.  
Ferramentas como o CURL fornecem opções de linha de código.

{% hint style="info" %}
Você deverá salvar as suas chaves de API, independentemente de qualquer coisa. NÃO COMPARTILHE suas chaves de API com ninguém, nem mesmo nos canais de suporte da Zoop. Nenhum funcionário da Zoop está autorizado a pedir sua chave de API ou qualquer outro dado sensível!
{% endhint %}

